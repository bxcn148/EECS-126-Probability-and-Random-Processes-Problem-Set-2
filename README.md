Download link :https://programming.engineering/product/eecs-126-probability-and-random-processes-problem-set-2/


# EECS-126-Probability-and-Random-Processes-Problem-Set-2
EECS 126: Probability and Random Processes Problem Set 2
1. Among Us

In the game of Among Us, there are 9 players. 4 of them are imposters and 5 of them are crewmates. There is also a deck of 17 cards containing 11 \sabotage” cards and 6 \task” cards. Imposters want to play sabotage cards, and crewmates want to play task cards. Here’s how the play proceeds.

A captain and a rst mate are chosen uniformly at random from the 9 players.

The captain draws 3 cards from the deck and gives 2 to the rst mate, discarding the third.

The rst mate chooses one to play.

Now suppose you are the rst mate, but the captain gave you 2 sabotage cards. Being a crewmate, you wonder, did the captain just happen to have 3 sabotage cards, or was the captain an imposter who secretly discarded a task card. In this scenario, what’s the probability that the captain is an imposter? Let’s assume that imposter captains always try to discard task cards, and crewmate captains always try to discard sabotage cards.

2. Lightbulbs

Consider an n n array of switches. Each row i of switches corresponds to a single lightbulb Li, so that Li lights up if at least i switches in row i are ipped on. All of the switches start in the \o ” position, and each are ipped \on” with probability p, independently of all others. What is the expected number of lightbulbs that will be lit up? Express your answer in closed form without any summations.

3. Compact Arrays

Consider an array of n entries, where n is a positive integer. Each entry is chosen uniformly randomly from f0; : : : ; 9g. We want to make the array more compact, by putting all of the non-zero entries together at the front of the array. As an example, suppose we have the array

[6; 4; 0; 0; 5; 3; 0; 5; 1; 3]:

After making the array compact, it now looks like

[6; 4; 5; 3; 5; 1; 3; 0; 0; 0]:

Let i be a xed positive integer in f1; : : : ; ng. Suppose that the ith entry of the array is non-zero (assume that the array is indexed starting from 1). Let X be a random variable which is equal to the index that the ith entry has been moved after making the array compact. Calculate E[X] and var(X).


4. Borel-Cantelli & Strong Law

In this problem, we walk through a proof of the strong law (assuming nite 4th moments) that relies only on basic probability. In class we covered the Borel-Cantelli lemma, which

states that for events (An)1

P

1

P (An i.o.) = 0;

, if

P (An) <

1

, then

n=1

n=1

where we de ne the event fAn i.o.g = \n 1 [m n An as the event where in nitely many An occur.

Let X1; X2; : : : be i.i.d. with EXi = 0 and EXi4 < 1 (and so we also have nite second and third moments). Let Sn = X1 + + Xn, and compute E[Sn4]. Write your answer in terms of the moments E[Xi2]; E[Xi3]; E[Xi4].

Fix an > 0, and use Markov’s inequality to show that, for any n,

P (jSn=nj > ) O(n 2):

Finally, use Borel-Cantelli to conclude that P (limn!1 Sn=n = 0) = 1. This a weaker (the full theorem assumes only nite rst moments) form of the strong law of large numbers.

5. Bounds for the Coupon Collector’s Problem

Recall the coupon collector’s problem, where each box contains a single coupon, and there are n di erent types of coupons. We let X be a random variable which is equal to the number of boxes bought until one of every type of coupon is obtained.

The expected value of X is nHn, where Hn is the harmonic number of order n which is de ned as

n

1

Hn =

Xi

;

i

=1

and satis es the inequalities

ln n Hn ln n + 1:

(a) Use Markov’s inequality in order to show that

1

P (X > 2nHn) 2:

(b) Use Chebyshev’s inequality in order to show that

2

P (X > 2nHn) 6(ln n)2 :

Note: You can use the identity

1 1 2

X

i2 = 6 :

i=1

(c) De ne appropriate events and use the union bound in order to show that

1

P (X > 2nHn) n:

Note: The sequence an = (1 1=n)n, for n = 1; 2; 3; : : :, is strictly increasing and limn!1 an = 1=e.
