# polkadot binary does not work on 'armhf',
# so this must be run on a more expensive 'X86' server ...

# using extra storage, mounted to /mnt/extradisk/, see
# computer/Linux/mount-a-blockdevice.txt

apt install wget
mkdir polkadot; cd polkadot
wget https://github.com/paritytech/polkadot/releases/download/v0.8.25/polkadot
chmod 755 polkadot
mkdir /mnt/extradisk/blockchains

nano ./run-polkadot.sh
######################
NODENAME="infunity"
STORAGEPATH=/mnt/extradisk/blockchains/
CHAIN=polkadot
LOGFILE=polkadot-$CHAIN-$NODENAME.log

./polkadot --chain=$CHAIN --base-path $STORAGEPATH --wasm-execution=compiled --name $NODENAME --telemetry-url "wss://telemetry.polkadot.io/submit/ 5" &> $LOGFILE &

echo
echo node is running, in the background. Now check logfile:
echo tail -f $LOGFILE
######################

# keep eye on disks:
watch -n 5 "du /mnt/extradisk/blockchains/chains/polkadot -d 0; df -h | grep 'extradisk\|vda1'"

# when ready, search for $NODENAME and screenshot at
#           https://telemetry.polkadot.io/#/Polkadot 

