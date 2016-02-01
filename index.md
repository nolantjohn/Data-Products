---
title       : Generation Guesser
subtitle    : Predicting Your Generation
author      : Nolan
job         : Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

- This application attempts to guess what generation a user belongs to
- Generation Breakdown:

```r
gendata <- read.csv("data/generationrangdata.txt")
gendata
```

```
##     generation minAge maxAge
## 1  Baby Boomer     50     70
## 2 Generation X     36     49
## 3   Millenials     18     35
```

---

## Pitch?

- The motivation behind this app is two fold:

        1. I was interested in seeing what age group of users would find and use this app the most
        
        2. I wanted to know if certain generations are more aware of their 
           generation's characteristics then others
        
- This app was put together quickly, so the questions are items that came to mind over a week period
- By using the app your are helping create data points that will hopefully answer the questions above
- Give it a try, it'll only take a minute

---

## Inputs & Outputs

Inputs:

- General questions answered through true or false check boxes
- Drop down list taking in the users actual generation
- The ability to save the users session data (guess, real generation, and if they know their generation)

Outputs:

- The generation guessed
- Whether or not the guess was correct
- A plot of the applications use by generation

---

## Usage to Date


```r
gendata <- read.csv("data/generationdata.csv")
plot(gendata$Answer, main = "Usage by Generation")
```

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png)






