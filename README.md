## Confidence Interval on a Proportion

+ You flick a tack 50 times and finds that it points up 18 times.  Being a
budding statistician, you readily compute a 95% confidence interval on the
probability that the tack points up using the usual STAT 121 formula:
![equation](https://latex.codecogs.com/gif.latex?%5Chat%7Bp%7D%20%5Cpm%201.96%20%5Csqrt%7B%5Chat%7Bp%7D%281-%5Chat%7Bp%7D%29/n%7D)
where n=50 and, for the data you collected,
![equation](https://latex.codecogs.com/gif.latex?%5Chat%7Bp%7D%3D18/50) so the
confidence interval is (0.23,0.49).

+ You then recall that this confidence interval procedure is based on a
central limit theorem which assumes a large sample size.  Thus, despite being
named a "95% confidence interval," the procedure may not have 95% coverage in
finite (e.g., n=50) samples.  What is the coverage of this confidence 
interval procedure if the actual probability that the tack points up is 0.4? 
Remember to assess your Monte Carlo error!  Solve the problem by performing a 
simulation study in an R script called `tack.R` (or `tack.Rmd`).

## "Let's Make a Deal"

+ Wikipedia provides context for this problem, known as the [Monty Hall 
Problem](https://en.wikipedia.org/wiki/Monty_Hall_problem).

+ Essentially, the idea is this: You're on a game show and you are presented
with 3 doors. Behind one door is a fabulous grand prize (let's say it's a 
new car so you no longer have to deal with the UVX bus). Behind the other two
doors are less fabulous prizes (for fun, let's say each of the other two 
doors is concealing an old goat). You're goal, obviously, is to select the 
door concealing the car.

+ To start the game, you select a door you believe is concealing the grand
prize. The show host then opens one of the remaining doors, revealing an
old goat. You now have the option to either stick with your initial choice, 
or select the other remaining door.

+ This question was posed to the "Ask Marilyn" column of *Parade* magazine in 
1990 as follows:

    *"Suppose you're on a game show, and you're given the choice of three doors: 
Behind one door is a car; behind the others, goats. You pick a door, say No.
1, and the host, who knows what's behind the other doors, opens another door, 
say No. 3, which has a goat. He then says to you, 'Do you want to pick door 
No. 2?' Is it to your advantage to take the switch?"*

+ The answer given by Marilyn von Savant (author of the Ask Marilyn column) 
was that the contestant should switch to the other door. Nearly 10,000 readers
responded to this response, many of them claiming it was incorrect.

+ Your task consists of arguing empirically whether Marilyn Vos Savant is 
correct. In an R script named `deal.R` (or `deal.Rmd`), write a simulation 
study that replicates the game show as much as possible (i.e., randomly 
choosing doors, etc.). Implement both strategies (i.e., "do not switch" versus 
"switch").  Give the probability of winning under each of the strategies. 
Quantify your uncertainity about the emperically estimated probabilities by 
forming a confidence intervals on the proportions of wins.

**There is no additional step necessary to turn in your homework. Simply create
the scripts described above and save your work in RStudio Cloud. Remember not
to edit or access your homework after the due date or it may be considered a
late submission.**