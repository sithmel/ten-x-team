## how to be a 10x team

@sithmel

Note:
I have made these mistakes, you don't have to
---
How to measure if a team is successful?
---
A successful team delivers a great product
and keeps delivering on a constant pace
---
## Delivering a great product
---
Set the right priorities
* sort by certainty <!-- .element: class="fragment" data-fragment-index="1" -->
* delay what you can <!-- .element: class="fragment" data-fragment-index="2" -->
* UI/UX before backend <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
Reprioritise tasks in order of certainty.
Delay all decisions that can be delayed
Start with the frontend
---
Short development iterations:

* refactor to introduce new feature
* introduce feature + test
* integrate
* ship

Note:
Development iterations are not the same as product iterations.
I recommend super short iterations:

rules:
every day you ship a working version of the software
never build more features then expected but keep the system open to add new features

---
> "If you want to go fast, go alone. If you want to go far, go together."

African Proverb
---
Collaborate:
* resilience <!-- .element: class="fragment" data-fragment-index="1" -->
* sharing and learning <!-- .element: class="fragment" data-fragment-index="2" -->
* for sanity check <!-- .element: class="fragment" data-fragment-index="3" -->
---
How?
* Pairing/Mobbing <!-- .element: class="fragment" data-fragment-index="1" -->
* Show and tell <!-- .element: class="fragment" data-fragment-index="2" -->
* Knowledge sharing <!-- .element: class="fragment" data-fragment-index="3" -->
* Code reviews <!-- .element: class="fragment" data-fragment-index="4" -->

Note:
PRs:
only when necessary
* unsure, or needs validation
* show and tell
* push to master otherwise
* PR ARE A BLUNT TOOL FOR ENSURING CORRECTNESS
---
### Testing

Note:
never postpone testing
Test is supposed to help you, should not be a chore.
Automated tests should save your time 
If testing is difficult consider changing the code or changing testing strategy/level.
100% test coverage is often the wrong goal
try to cover 1 obvious cases and the corner cases
balance cost/convenience
---
## A successful team keeps delivering on a costant pace
Note: Let's focus on the second part
---
> "Legacy software is any software where people are afraid to make changes”

Rajiv Prabhakar
Note:
How to maintain a project approachable and easy to understand ?
---
Tech debt
- only if necessary <!-- .element: class="fragment" data-fragment-index="1" -->
- documented <!-- .element: class="fragment" data-fragment-index="2" -->
- two types <!-- .element: class="fragment" data-fragment-index="3" -->
---
> “Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live”

John Woods

Note:
I am trying to stick to this principle, and for this reason I don't give anyone my address
---
document:
- how <!-- .element: class="fragment" data-fragment-index="1" -->
- why <!-- .element: class="fragment" data-fragment-index="2" -->
- tradeoffs <!-- .element: class="fragment" data-fragment-index="3" -->
- assumptions <!-- .element: class="fragment" data-fragment-index="4" -->
- tech debt <!-- .element: class="fragment" data-fragment-index="5" -->

Note:
- document your love for the next dev. document why, tradeoffs, assumptions, tech debt
---
- a service should talk with itself
- fake endpoint to external services when practical
- create demo page
- fake the data (for test and demo)
- when refactoring, get rid of unused code and packages
---
Don't be too clever
- Vanilla is better (keep things simple and do not use fancy libs, unless necessary or very convenient)
- do not use nesting on sass. Except for namespacing
- do not use fancy transpilation or macros
- use functional paradygm with moderation
- use rest sensibly, graphql is probably not the solution you are looking for
- explicit is better than implicit. Use the minimal amount of things you need and do not over-engineer
---
solve the problem for everybody
---
Be proud of what you achieve

