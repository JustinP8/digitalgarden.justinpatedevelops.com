---
title: "Feature Development Checklist"
date: 2022-05-03T12:32:59-05:00
tags: ["seedling", "software-development", "unit-testing", "security", "lists", "check-list"]
categories: ["career"]
#series: []
---
Whenever developing a new feature at work, what follows is a list of things a developer should keep in mind and follow up on before calling a feature complete. Arguably, each bit of work (e.g. a user story) should also address these things as you work on a larger feature that is encompassed by an epic (i.e. a feature spanning the completion of multiple user stories).

* Are the acceptance criteria met?
* Is it secure?
  * Does it expose any personal information (e.g. Personal Identifying Information (PII), Personal Health Information (PHI), etc.)
  * No SQL injection concerns
  * No cross-site scripting vulnerabilities
  * todo: list out more of the OWASP vulnerabilities to prevent
* Are all inputs validated?
  * Are appropriate error messages returned for invalid input?
* Is functional access verified?
  * Are users prevented from performing functions that their security group does not allow?
* Is appropriate testing in place?
  * Is code covered acceptably with Unit Tests?
  * Is appropriate integration testing built (testing integration with databases, APIs, third parties, etc.)?
  * Have load tests been put in place, if applicable?
* Does the feature consider accessibility?
  * Can a person with a permanent, situational, or temporary disability use the feature? This includes things like:
    * Keyboard navigation and shortcuts
    * Screen reader optimizations
    * Good visual contrast
    * Filling in colors with patterns to help with contrast in visuals for those with color-blindness
