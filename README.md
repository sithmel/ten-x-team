## how to be a 10x team
A reflection
<!-- .slide: data-background="./imgs/closeup-photo-of-primate-1207875.jpg" -->

Maurizio Lupo

---
What makes an **engineering** team successful?
---
Delivering with **increased** velocity over time
---
## Delivering
<!-- .slide: data-background="./imgs/lucian-alexe-1MUBZt4zoJ0-unsplash.jpg" -->
---
Dealing with uncertainty
* start doing what you are sure of <!-- .element: class="fragment" data-fragment-index="1" -->
* delaying decision point <!-- .element: class="fragment" data-fragment-index="2" -->
* start with the user <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
accept that things are going to change

What are the right priorities

Reprioritise tasks in order of certainty.

Delay all decisions that can be delayed

Start with the frontend, or api. Start with "the consumer"
---
Short **development** iterations:

1. refactor to introduce new feature <!-- .element: class="fragment" data-fragment-index="1" -->
2. introduce feature + test <!-- .element: class="fragment" data-fragment-index="2" -->
3. integrate <!-- .element: class="fragment" data-fragment-index="3" -->
4. ship <!-- .element: class="fragment" data-fragment-index="4" -->
5. goto 1 <!-- .element: class="fragment" data-fragment-index="5" -->

Note:
Development iterations are not the same as product iterations.

I recommend super short iterations. (1 day)

rules:

every day you ship a working version of the software

never build more features then expected but keep the system open to add new features

The process requires that, when thinking how to go from A to B. You have to consider the journey, not only the final result.
---
<!-- .slide: data-background="./imgs/ape-monkey-monkey-family-affchen-66865.jpg" -->
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
* Code reviews <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
PRs with purpose (unsure, or needs validation, show and tell)

* push to master otherwise

* PR ARE A BLUNT TOOL FOR ENSURING CORRECTNESS
---
Engineer toolkit
* SOLID <!-- .element: class="fragment" data-fragment-index="1" -->
* Design patterns <!-- .element: class="fragment" data-fragment-index="2" -->
* Data structure and analysis <!-- .element: class="fragment" data-fragment-index="3" -->
* Functional concepts <!-- .element: class="fragment" data-fragment-index="4" -->
* ... <!-- .element: class="fragment" data-fragment-index="5" -->

Note:

---
### The testing pyramid
<!-- .slide: data-background="./imgs/pyramid.png" -->
---
### Unit tests
* Never postpone <!-- .element: class="fragment" data-fragment-index="1" -->
* it is code scaffolding <!-- .element: class="fragment" data-fragment-index="2" -->
* good code is easy to test <!-- .element: class="fragment" data-fragment-index="3" -->
* easy to write and to delete <!-- .element: class="fragment" data-fragment-index="4" -->

Note:
Never postpone testing: test is supposed to help you, should not be a chore.
Automated tests should save your time. But the only do so if you don't postpone them.

If testing is difficult consider changing the code or changing testing strategy/level.

100% test coverage is often the wrong goal

try to cover 1 obvious cases and the corner cases
balance cost/convenience

---
### Other tests
* the only "end-to-end tests" fallacy <!-- .element: class="fragment" data-fragment-index="1" -->
* beware of slow tests <!-- .element: class="fragment" data-fragment-index="2" -->
* happy path  <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
Balance for acceptance and unit test:
"I don't need to write unit test because I am experienced enough to write modular/testable code. Also testing the implementation may become an hindrance when refactoring.
I only need to write acceptance test to ensure the correctness"
Unit tests: quick to write and to throw away
tests purpose is to speed development
---
## Increase velocity
<!-- .slide: data-background="./imgs/yellow-bananas-61127.jpg" -->

Note: Let's focus on the second part
---
<!-- .slide: data-background="./imgs/building-with-tree-1534057.jpg" -->
> "Legacy software is any software where people are afraid to make changes”

Rajiv Prabhakar
Note:
If people are afraid, they are not refactoring and the code deteriorates.
When this happen the development slows down considerably.

How to maintain a project approachable and easy to understand ?
---
*"Technical debt in software design is the implied cost of future reworking because a solution prioritizes expedience over long-term design."*

Note:
In simpler words if you have a tech debt in a certain part of the code/architecture, it takes a longer time to change/evolve that part of the code.
---
Tech debt
- only if necessary <!-- .element: class="fragment" data-fragment-index="1" -->
- documented <!-- .element: class="fragment" data-fragment-index="2" -->
- two types <!-- .element: class="fragment" data-fragment-index="3" -->
Note: 

There are 2 types of tech debt. The first one can be addressed the first time you change the code (as soon as it is documented clearly). I suggest to document it in the codebase, so that the next person making a change will pick it up.

The second type takes more effort and time and requires planning ahead. You have to deal with this and agree a strategy with the PM.
---
<!-- .slide: data-background="./imgs/gorilla-animal-35992.jpg" -->

> “Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live”

John Woods

Note:

I am trying to stick to this principle, and for this reason I don't give anyone my address
---
Document:
- how (to run/to test/to use) <!-- .element: class="fragment" data-fragment-index="1" -->
- why <!-- .element: class="fragment" data-fragment-index="2" -->
- tradeoffs <!-- .element: class="fragment" data-fragment-index="3" -->
- assumptions <!-- .element: class="fragment" data-fragment-index="4" -->

Note:
- document your love for the next dev. document why, tradeoffs, assumptions, tech debt
keep the documentation in the most obvious place and keep it up-to-date.

---
Keep it simple
- Consider maintenance cost at every step <!-- .element: class="fragment" data-fragment-index="1" -->
- "everybody does it" is no good reason <!-- .element: class="fragment" data-fragment-index="2" -->
- don't be too clever <!-- .element: class="fragment" data-fragment-index="3" -->
- explicit is better than implicit <!-- .element: class="fragment" data-fragment-index="4" -->
- do not look too far ahead <!-- .element: class="fragment" data-fragment-index="5" -->

Note: 
Examples
- Vanilla is better (keep things simple and do not use fancy libs, unless necessary or very convenient)
- do things for a reason
- use functional paradygm with moderation
- use rest sensibly, graphql is probably not the solution you are looking for
- do not use nesting on sass. Except for namespacing
- do not use fancy transpilation or macros

Use the minimal amount of things you need and do not over-engineer
---
Not finished unless:
- Observability (including alerting) <!-- .element: class="fragment" data-fragment-index="1" -->
- Logs <!-- .element: class="fragment" data-fragment-index="2" -->
- Manageable (Admin UI or tooling) <!-- .element: class="fragment" data-fragment-index="3" -->
- Audit <!-- .element: class="fragment" data-fragment-index="4" -->
- Business metrics <!-- .element: class="fragment" data-fragment-index="5" -->
- Scalable and resilient <!-- .element: class="fragment" data-fragment-index="6" -->

Note: 
dedicate time and attention on monitoring, alerting, audit, debugging helpers
 (no manual data operation allowed)
---
## Solve a problem once
<!-- .slide: data-background="./imgs/view-ape-thinking-primate-33535.jpg" -->
Note: 
when you work on something think if it can be generalised and reused in other cases
---
## Be proud of what you achieve
<!-- .slide: data-background="./imgs/brown-primate-hanging-on-tree-1123771.jpg" -->
---
## Thanks
<!-- .slide: data-background="./imgs/black-chimpanzee-smiling-50582.jpg" -->
* @sithmel@fosstodon.org
* maurizio.lupo@gmail.com
