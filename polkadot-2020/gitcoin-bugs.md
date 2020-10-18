# polkadot 2020 hackathon
## gitcoin bugs

Sorry to have had a suboptimal experience here. In this case it is really not so important, because the amounts of money are tiny, and the whole thing is mainly just for fun; probably good to try out gitcoin for a toy situation like this.  However, it was a bit frustrating - I have put work in, and then submitting it kept on failing. 

I do not know whether the problems are caused by polkadot (the hackathon organizer) or by gitcoin (the bounties platform). Skim through it, probably you know better than me to whom to forward this who could actually do something about it.

... 

New to gitcoin, so I might not have really understood what to do exactly. If all this here was my fault indeed, then please still have a 2nd look at your own system ... how you could make it easier for newbs to grasp it intuitively. Thanks a lot. May this then help to give an outside perspective.

Having spent all day with this, and then not being able to submit my work was a bit frustrating, especially because the number of bounties is so limited; so I felt I was competing with others to be ready QUICKLY enough, not to end up without any bounty.  
Here is actually one way out, in such a beta system situation: Offer MORE bounties than just 50, to reduce the stress.

Yes, my main intention is to try out gitcoin, and look around how polkadot created this hackathon, but the new money IS an incentive indeed. Another suggestion: Raise the tiny value of the bounties?

What do you think?
   

### bug 1: cannot submit

>  "Unable to fulfill bounty. Please try again later"

NOT a helpful error message. 

WHY is the system 'unable'?   
And what if 'later' the problem is still there?  
And in my case here, the second part would not have helped: 
 
Much later, via the discord chat, I found out that the FORM ITSELF has a bug \*sigh\*: fractions of an hour (e.g. 0.5) are not allowed? See https://github.com/gitcoinco/web/issues/7695 if that is the case, then the frontend must disallow that, right?

Then when using "1" hours, I did NOT get the same error message. Hooray. So I suppose, my work is submitted now?  *How would I know?*

Oh yes, patience until the system updates was another suggestion - I have now waited approx 1 hour, is that perhaps not long enough?  Give an approximate/minimum/maximum waiting time please.


### bug 2: no user feedback whatsoever
*Have I submitted?*  
*Have I not submitted?*   

**How would I know that?**

The [dashboard](https://gitcoin.co/dashboard) still has the "Submit work" button **enabled** for my challenges in "Bounties in Progress", *as if I still have to* submit my work.

But then when trying that (again), the same error message again:

>  "Unable to fulfill bounty. Please try again later"

Which in this case now is not only not helpful, but really ... wrong.

(Only) using the console (thx chat, great idea), I found this error message:

> "raven.js:58 error: bounty fulfillment failed with status: 400 and message: error: user can submit once per bounty"

That looks as if I HAD submitted my work? Good. Happy. (Finding that out via the console, lol.)


#### Suggestions:
Think about ALL the ways, that "submit work" can fail, and treat them *differently*.

Show an accurate error message.   
Show a correct error message.  
Show a helpful error message.  
And not only in the console.

Show a clear "success" message, once the thing actually goes through. And there tell us, how long to wait now min/avg/max - and then to check which URL.

Plus, what about using the section on the [dashboard](https://gitcoin.co/dashboard) which right now says "zero Work Submitted", and "You don't have any submission awaiting payment". 

What if you let it instead express something like: "You have submitted 2 pieces of work, in approx 48 hours someone will look at it.". 

#### EDIT: profile ... not dashboard

Hah, found something ... elsewhere: The "profile".

So the "dashboard" is broken/incomplete, but the "[profile](https://gitcoin.co/drandreaskrueger)" does actually contain some information that I had been hoping for. There I can see that my submitted work was received. Ahhh, what a relief. 

Great.

--> 

Idea: Explain it with a sentence "this is the dashboard, here you can NOT see blablabla, i.e. --> go to the profile instead"

Or even: Better completely disable the "dashboard"?



### perhaps it's me who is the problem here?

Then please explain where my conceptual misunderstanding is. Thanks.

One more thing: (Why) Do I still have to press "Stop work", even after having submitted my work?

  