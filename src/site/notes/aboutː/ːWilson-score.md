---
{"dg-publish":true,"permalink":"/about/wilson-score/","dgPassFrontmatter":true}
---

roll a d20 once and get a 1.
Is it weighted? Probably not, it could still be totally fair,
it's a $5\%$ chance, and getting a bad $5\%$ chance once is totally normal
So we accept that


Now we take a coin, it's weighted, but how weighted?
We flip it 12 times, and get 0 heads.
Is it weighted to always be tails? Maybe.
But what if there was 20 parallel universes,
and we just happen to be in the 1 that got all tails?

That's a $5\%$ chance, the same as our non suspicious d20,
so lets say if an event happens $5\%$ of the time, then us observing it isn't once isn't weird or abnormal, even if it is unlucky

We can then calculate how likely tails has to be so that 12 tails has a $5\%$ chance, which gives us how unlikely tails could be and we still have at least a $5\%$ chance of getting 12.

The chance of getting 12 tails in a row is $p^{12}$, where $p$ is the chance of 1 tails
If we solve this for a probability of $5\%$ we get $p=\sqrt[12]{0.05}$ which is $\approx78\%$
Which is far off what a naive guess of just looking at how many tails appeared would give us (Which would be $100\%$). We hence say that the actual chance the coin gives tails is $\left[78\%, 100\%\right]$ (With a $95\%$ confidence)

This is just a rough overview, in reality a more complicated formula know as the Wilson Score interval is used to give a more accurate answer, but this shows how a naive guess of "it is always tails" is wrong.

If we were continue to flip the coin and always see tails then the lower $78\%$ bound on our estimate would rise, with 24 trails we get $88\%$. 48 trails gives $93\%$, doubling the number of trails roughly halves the distance to $100\%$