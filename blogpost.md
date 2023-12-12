## What is validation
Simply put, validation is the act of documenting evidence that a system meets a pre-specified set of expectations. This means that off-the-shelf software does not come pre-validated. Furthermore, any software can be validated, given you have the resources to do so. 

There is also a sentiment that open source software cannot be validated, because it can be changed by anyone. While it is true that open source software can be modified by anyone, this does not mean that official sources of OS software have to accept or incorporate someone's changes. In fact many validated systems have built on open source software for many years if not decades (e.g. linux, mysql, etc.) Furthermore, once installed, OS software is just as secure as propriatary software in terms of access to binaries etc.

21 CFR Part 11 is the rule that is referenced as governing electronic system validation. However, 21CFR Part 11, I think it was written with a focus on data collection and storage and not analysis. 

## How do you validate a system

Validaiting a system usually has the following steps. 
1) Generate user, functional, design requirements.
2) Perform a risk assessment
2) Generate functional and design specifications.
3) Map requirements to specifications.
4) Create test cases to cover requirements
3) design the system.
4) build system
5) test system and capture evidence of successful test case execution
6) deploy to production environment.

### What can('t) you validate?
You cannot validate a system with out a use case. The use case could be broad: "A user must be able to perform statistical calculations with data. It could be narrow: "The system must serve an API endpoint that calculates the mean of upto 250 numbers with to the 7th decimal place." A system, will usually have many user requirements, ranging from end user requirements to lower level infrastructure requirements, e.g. user/netowrk authentication, data encryption etc.

### Can you validate a language?
We cannot validated a language (e.g. R, Python, SAS, etc). We can validate the language's interpreter. For example, in R does `hist(rnorm(100, 1,0))` generate histogram plot? 


## What do you actually validate?


## How does risk come into play with validation
  We cannot test everything. Some of our expectations are implicit and some are explicit.
  We test more when system failure causes more damage (e.g. patient death, patient harm, everything else).

## What do we really care about w.r.t. validation

### Statistician
  Functions/methods are numerically accurate, e.g. the right answer, a.k.a. accuracy 2+2 = 4. This group generally is not concerned with formal documentation of test case execution. This group also tends to trust commerical software over OS source software. 

### Quality
  Change management control. Who, what, why and when the system was changed. Change management control against a broad set of requirements, i.e. user authentication, end-user requirements/expectations. This group almost doesn't care about what Statisticans/analysts care about. That is to say, if a user requirement stats that the system must compute 2+2=5. So long as that expectation can be met then the sytem can be validated. Furthermore, 

### The FDA

#### Statistical Review
  Statisical reviewers care about the same thing other statisticians care about, the right method for the right analysis. In general, they are less worried about change management.

#### Audit Inspection team
  Regulatory auditors care about the same things a companies quality groups cares about: robust documentation of change management and access controls, etc. They do not care so much about whether a method or package is the right one so long as there is documentation surrounding its addition/modificaton in the environment. 

