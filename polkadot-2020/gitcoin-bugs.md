# polkadot 2020 hackathon
## gitcoin bugs

It was a suboptimal experience, really.

I do not know whether the problems are caused by polkadot or by gitcoin. And I am very new to gitcoin, so I might not have really understood what to do exactly. If all this here was my fault indeed, then please have a second look at your own system how you could make it easier for newbs to start using it. Thanks a lot.

I have spent all day with this, and to not be able to submit my work was a bit frustrating, especially because you limited the number of bounties, so I felt I was competing with others to be ready quickly enough, not to end up without any bounty.

I think that is actually a way out, in such a beta system: Just offer MORE bounties than just 50, to reduce the stress.

What do you think?
   

### bug 1: cannot submit

>  "Unable to fulfill bounty. Please try again later"

Which is NOT a helpful error message. WHY is the system unable? And what if "later" the problem is still there?
 

Much later, via the discord chat, I found out that the FORM ITSELF has a bug *sigh*: fractions of an hour (e.g. 0.5) are not allowed.

Then when using "1" hours, I did NOT get the same error message.

So I suppose, my work is submitted now?

How would I know now?

Oh yes, patience - I have now waited approx 1 hour, is that perhaps not long enough???


### bug 2: no user feedback whatsoever
*Have I submitted?*  
*Have I not submitted?*   

**How would I know that?**

The [dashboard](https://gitcoin.co/dashboard) still has the "Submit work" button enabled for my challenges "Bounties in Progress", *as if I still have to* submit my work.

But then when trying that (again), the same error message again:

>  "Unable to fulfill bounty. Please try again later"

Which in this case now is not only not helpful, but really ... wrong.

(Only) using the console (thx chat, great idea), I found this error message:

> "raven.js:58 error: bounty fulfillment failed with status: 400 and message: error: user can submit once per bounty"

That looks as if I HAD submitted my work? Good.


#### Suggestions:

Show an accurate error message.   
Show a correct error message.  
Show a helpful error message.  
Not only in the console, no.    

What about using the section on the [dashboard](https://gitcoin.co/dashboard) which right now says "Work Submitted", and "You don't have any submission awaiting payment" 

What if you let it instead express something like: "You have submitted 2 pieces of work". 

Wouldn't that be nice?

#### EDIT: profile ... not dashboard

Hah, found something ... elsewhere:

So the "dashboard" is broken/incomplete, but the "[profile](https://gitcoin.co/drandreaskrueger)" does actually contain the information that I had been hoping for. There I can see that I have submitted my work. Ahhh, what a relief. 

Great.

--> 

Idea: Explain it with a sentence "this is the dashboard, here you can NOT see blablabla, i.e. --> go to the profile instead"

Or: Better completely disable the "dashboard"?



### perhaps it's me who is the problem here?

Then please explain where my conceptual misunderstanding is. Thanks.

One more thing: (Why) Do I have to press "Stop work", after having submitted my work?

  