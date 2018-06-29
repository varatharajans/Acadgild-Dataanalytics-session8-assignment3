# Acadgild-Dataanalytics-session8-assignment3
DATA ANALYTICS WITH R, EXCEL AND TABLEAU SESSION 8ASSIGNMENT 3
session1 assignment 3 probabiity
varatharajan
June 21, 2018

1. A recent national study showed that approximately 44.7% of college students have used Wikipedia as a source in at least one of their term papers. Let X equal the number of students in a random sample of 
size n = 31 who have used Wikipedia as a source. 
Perform the below functions 
a. Find the probability that X is equal to 17 
b. Find the probability that X is at most 13 
c. Find the probability that X is bigger than 11. 
d. Find the probability that X is at least 15. 
e. Find the probability that X is between 16 and 19, inclusive

How is X DISTRIBUTED?

X~binom (size=31, probability=0.447)

## x ~ binom(size = 31, probability = 0.447)

#Find the probability x=17

dbinom(17,size=31,prob=0.447)
## [1] 0.07532248
b. Find the probability that X is at most 13 ?

pbinom(13, size=31,prob=0.447)
## [1] 0.451357
c. Find the probability that X is bigger than 11. ?

pbinom(11, size=31,prob=0.447, lower.tail = FALSE)
## [1] 0.8020339

d. Find the probability that X is at least 15. ?

pbinom(14, size=31,prob=0.447, lower.tail=FALSE)
## [1] 0.406024

e. Find the probability that X is between 16 and 19, inclusive?

sum(dbinom(16:19, size=31,prob=0.447,))
## [1] 0.2544758
diff(pbinom(c(19,15),size=31,prob=0.447, lower.tail = FALSE))
## [1] 0.2544758



title: "session1 assignment 3 probabiity"
author: "varatharajan"
date: "June 21, 2018"
output: word_document
---
```{r}
x~binom(size=31,prob=0.447)
#Find the probability x=17
dbinom(17,size=31,prob=0.447)
pbinom(13, size=31,prob=0.447)
pbinom(11, size=31,prob=0.447, lower.tail = FALSE)
pbinom(14, size=31,prob=0.447, lower.tail=FALSE)
sum(dbinom(16:19, size=31,prob=0.447,))
diff(pbinom(c(19,15),size=31,prob=0.447, lower.tail = FALSE))
x ~ binom(size = 31, prob = 0.447)
[1] 0.07532248
[1] 0.451357
[1] 0.8020339
[1] 0.406024
[1] 0.2544758
[1] 0.2544758



```
