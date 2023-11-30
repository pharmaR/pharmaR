## What is validation
Simply put, validation is the act of documenting evidence that a system meets a pre-specified set of expectations.

21 CFR Part 11 is the rule that is referenced as governing electronic system validation. However, 21CFR Part 11, I think it was written with a focus on data collection and storage and not analysis. 

### To an analyst/statistician/data scientist
Functions/methods are numerically accurate

### To quality profession
Change management control against a broad set of requirements, i.e. user authentication, end-user requirements/expectations.

## What can('t) you validate?
You cannot validate with out a use case. 

### Can you validate a language?
We cannot validated a language (e.g. R, Python, SAS, etc). We can validate the language's interpreter. For example, in R does `hist(rnorm(100, 1,0))` generate histogram plot. 


## What do you actually validate?


## How does risk come into play with validation
  We cannot test everything. Some of our expectations are implicit and some are explicit.
  We test more when system failure causes more damage (e.g. patient death, patient harm, everything else).

## What do we really care about w.r.t. validation

### Statistician
  The right answer, a.k.a. accuracy 2+2 = 4

### Quality
  Change management control. Who, what, why and when the system was changed

### The FDA
  Quality assurance

