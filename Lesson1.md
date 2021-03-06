---
title: "Week 1"
author: "Pablo Velásquez"
date: "15/2/2021"
output: 
  html_document: 
    keep_md: yes
---


 
## **Topics of the course** 
* Population 
* Sample 
* Design Studies 
* Scope
* EXploratory data analysis 
* Inferences

# **Data basics**  

## **Types of variables**      
 
### *Numerical*  

* Continuous: infinite number of values within a range
* Discrete: one specific set of numeric values

### *Categorical*  

* Ordinal: variable have inherent ordering
* Regular categorical: dont have order


## **Relationships between variables**   

two variables that show some connection with one another are called associated 
(dependent)

if the variables are not associated then are independent

## **Observational studies and experiments**       
   
### *Observational*        
  
Collect data in a way that does not directly interfere with how the data arise
  
With them you can only asses association -- causal inference methods (for the most part!)
   
### *Experiment*      

*Randomly assign* subject to treatments -- variation of the variable depends on the researcher

establish causal connection 

deals with the problem of **confounding variables**

**confounding variables:** Extraneous variables that affect both the explanatory and the response variable, and taht amke it seem like there is a realionship between them 


## **Sampling and sources of bias**       

Census is an impossibility

With a sample we can:

do an *Exploratory analysis*: Examine a part of the population to get an idea of the population as a whole

and as *inference study*: Generalized the idea to the population           
**To be validad** ----> sample needs to be representative 

### **Problem with samples: Sample bias**

* Convenience sample: individuals  who are easily accesible

* Non-response: if only a (non-random) fraction of the randomly sampled people respond to a survey susch that the sample is no loger representative of the population

* Voluntary response: Occurs when the sample consists of people who volunteer to respond

### **Sampling methods**

* **Simple random sample**: each case is equally likely to be selected
* **Sratified sample**: Divide the population into homogenous stata the randmly sample form within each stratum
* **Cluster sample**: Divide the population clusters, randomly sample a few clusters, then sample **all** observations within these clusters
* **Multistage sample**: Divide the population clusters, randomly sample a few clusters, then **randomly** sample all observations within these clusters.


## **Experimental Design**

* **Control**: Compare treatment to a control group 
* **Randomize**: Randomly assign subjects for treatment
* **Replicate**: Collect a sufficiently large sample, or replicate the entire study
* **Block**: Block variables know or suspected to affect the outcome

### **Blocking**

It is like **stratifying**, but instead of doing in the sampling part, is used in the random assignment part 

it can be used to determine if a treatment has different effects across different segments of the population 

### **Blocking vs. explanatory variables**

**Explanatory variables:** the treatment - the conditions that we can impose on experiment units

**Block variables:** Characteristics that the experimental units come with, that we would like to control.   

### **Blocking vs. explanatory variables**

**Placebo**
**Placebo effect**
**blinding**: experimental units dont know which group they are in 
**double-blind**: experimental units and researchers dont know the group of assignment 

## **Random sample assignment - Random assignment**

*Random sample assignment ---------------> Generalizability*

*Random assignment ----------------------> Causality*


