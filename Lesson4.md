---
title: "Lesson4"
output: 
  html_document: 
    keep_md: yes
---



 
## **Probability and distributions**

### **Random Process**

In a *Random Process* we know what outcomes could happen, but we don´t know which particular outcome will happen.  

### **Probability** 

***Notation***: P(A) = Probability of event A   

***Rule***: 0 <= P(A) <= 1

***Definition***:

* *Frequentist Interpretation*: The probability of an outcome is the proportion of times the outcome would occur if we observed the random process and infinite number of times.

* *Bayesian Interpretation*: A bayesian interprets probability as a subjective degree of belief. Popular in the late twenty years.

### **Law of large numbers** 

*Law of large numbers* states that as more observations are collected (more random process), the proportion of occurrences with a particular outcome converges to the probability of that outcome

<center>
*for example, we expect the Proportion of 5´s in a dice  to set down to 1/6 with increasing number of rolls*
</center>
<center>
![Proportion of 5´s v.s number of rolls](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\law of large numbers.PNG)
</center>

*Coin is memoryless*: The probability of heads on the 11th toss is the same as the probability of heads in the 10th toss, or any previous tosses
P(Head on the 11th toss) = P(Head on the 11th toss) = 0.5

*Gambler´s fallacy/law of averages*: Random processes are supposed to compensate for whatever happened in the past.... no, common misunderstanding of the law of large numbers


## **Disjoint Events + General Addition Rule**

### **Disjoint Events**  

*Disjoint Events* (Mutually exclusive) cannot happen at the same time.  
* A student can´t both fail and pass a class   
* A singe card drawn from a deck cannot be an ace and a queen    

<center>
*In Venn diagram, where we  represent each event by circles, if A and B are disjoint we end up with two circles that don´t touch each other*
</center>
<center>
![P](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\disjoint.PNG)
</center>

### **Non Disjoint Events**

*Non-Disjoint Events*  Can happen at  the same time    
* A student can get an A in Stats and A in Econ in the same semester  

<center>
*In Venn diagram,if A and B are non- disjoint we end up with two circles that join*
</center>
<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\nondis.PNG)
</center>

### **Union of Disjoint Events**

<center>
*Union: Probability of one event or the other happening*
</center>
<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\union.PNG)
</center>

### **Union of Non-Disjoint Events**

<center>
*We need to consider the join part of the two events in order to not double count and inflate our probability of a desire outcome*
</center>
<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\uniondis.PNG)
</center>

### **General addition rule**

<center>
P(A or B) = P(A) + P(B) - P(A and B)

and when the events are disjoint (P(A and B) = 0)..

P(A or B) = P(A) + P(B) 
</center>

### **Sample space**

A *Sample space* is a collection of all possible outcomes of a trial

</center>
<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\sampe.PNG)
</center>

### **Probability distribution**

A *Probability distribution* lists all possible outcomes in the sample space, and the probabilities with which thee occur

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\prodist.PNG)
</center>

**Rules**
* The events listed must be disjoint
* Each probability must be between 0 and 1
* The probability must total 1 (the sum)


### **Complementary events**

*Complementary events* are two mutually exclusive (disjoint) events whose probabilities add up to 1 

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\com.PNG)
</center>

### **Disjoint vs. complementary**

Do the sum probabilities of two disjoint outcomes always add up to 1?

**No** there may be more than 2 outcomes in the sample space 

## **Independence**

Two processes are *Independent* if knowing the outcome of one provides no useful information about the outcome of the other

* Outcomes of two tosses of a coin are *independent*
* Outcomes of two draws form a deck of cars (without replacement) are *dependent*

### **Checking for independence**

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\depen.PNG)
</center>

### **Example**

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\ex.PNG)
</center>

we use the expression **Most likely dependent** because we are dealing with sample data

If we observed difference between conditional probabilities (based in the sample) --> most likely dependent ---> Hypothesis test to see if this difference is not due to chance


### **Rules with independent events**

* **Product rule**

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\prod.PNG)
</center>

**Important Note** random selection implies independence 

----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
*Observation*: We can see a similarity between a dice roll and a sample

dice roll -- we know the 6 options and their relative frequencies (each option repeat only one time) --- if we roll the dice many times we get to the original relative frequencies.     
The 6 options and their relative frequencies is like a population that we don´t know -- if we take a sample of it we can get to the relative frequencies of the population  
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


## **Disjoint vs. Independent**


Disjointness is about events happening at the same time. While independence is about processes not affecting each other.


<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\ff.PNG)
</center>

**Note**: Disjoint events with non zero probability are always dependent on each other.Because if we know that one happened, we know that the other one cannot happen


<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\ff.PNG)
</center>

## **Conditional Probability**

## **Marginal Probability**

In a contingency table we look at the margins to calculate the marginal probabilities

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\margi.PNG)
</center>


## **Joint Probability**

In a contingency table we look at the intersection of the events of interest to calculate the joint probability. Also, in a Venn diagram we can see the joint probability as the intersection between the circles. 

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\joi.PNG)
</center>


## **Conditional Probability**


In a contingency table, we fix a column or row and only use the information registered on it.

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\cond.PNG)
</center>


In a formal way, we have the ***Baye´s Theorem***


<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\formu.PNG)
</center>


With this formula now **we can have an expression for the join probability of two events that are dependent**

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\nue.PNG)
</center>

## **Independence and conditional probabilities**

if two events are independent: P(A|B) = P(A)
***Conceptually***: Giving B doesn´t tell us anything about A
***Mathematically***: 
<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\math.PNG)
</center>

## **Probability trees**

See diapos

## **Bayesian Inference**

With probability trees we can calculate a *posterior probability*

**posterior probability: P(hypothesis|data)**: It tells us the probability of a hypothesis we set forth, given the data we just observed

depends on:

* Prior probability 
* Observed data 

This is different than what we calculated at the end of the randomization test on gender discrimination - the probability of observed or more extreme data given the null hypothesis being true, i.e. P(data|hypothesis) also called a p-value

In the bayesian approach, we evaluate claims iteratively as we collect more data.

In other words, we *update* our prior with our posterior probability from the previous iteration.

## **Example**

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\1.PNG)
</center>

<center>
![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\2.PNG)
</center>
<center>

![Pf](C:\Users\pablo\Desktop\Probability-and-Data-with-R\Images\3.PNG)
</center>

 
