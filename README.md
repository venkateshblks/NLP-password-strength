# Predict Password Strength using Natural Language Processing

**Password - 1000k unique values for password collected online**

**textStrength - three values(0 , 1 , 2) i.e. 0 for weak, 1 for medium, 2 for strong..
Strength of the password based on rules(such as containing digits, special symbols , etc.)**


**The passwords used in our analysis are from 000webhost leak that is available online**

## 1.. read data from SQL Database

## 2.. data cleaning

## 3.. Performing Semantic Analysis

### a) How many password textual actually holds only numeric characters ?

**only 26 people have set their password as only number**

### b) How many password textual actually holds only Upper-case character ?

**around 1500 users have their password as only capital letters**

### c) How many password textual actually holds only alphabet ?

**around 50 users have their password as alphabet letters only**

### d) How many password textual actually holds alpha-numeric character ?

**most of the users around 97K have their password as alpha-numeric..**

### e) How many password textual actually holds title-case character ?

**around 932 users have their password having first alphabet capital !**

### f) How many password textual actually holds special character ?

 **2663 observations have special characters in between them ..**

**2.6% people password actually uses special character in their password ..**

## 4.. Applying Feature Engineering

### Frequency of Lowercase Characters

### Frequency of Uppercase Characters

### Frequency of Numeric Characters

### Frequency of Special-case Characters

## 5.. Performing Descriptive Statistics

**Higher the length, Higher the strength**

**In case on alphabet frequency higher is not better.**

**Probably because it'll not be a strong password if max portion is occupied by just alphabets.**
**Password has more strength if the char types are spread in decent proportions**

## 6.. Feature Importance

**we have few overlappping region in distribution plot
when class is 2 , we have higher value of 'length' than class 1 & class 0
it means 'length' is a interesting feature as we have very less overlapping region
similarly from violinplot ,we will say on account of less overlappping ,
this feature 'length' is amazing & useful in determining the strength**

## 7.. Applying TF_IDF on data

## 8.. Applying Machine Learning algorithm

## 9.. Doing prediction on sample data (user-entered input)

## 10.. Model evaluation

