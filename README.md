## how to be a 10x team
A reflection
<!-- .slide: data-background="./imgs/closeup-photo-of-primate-1207875.jpg" -->

Maurizio Lupo

Note:
I have made these mistakes, you don't have to
---
How to measure if an engineering team is successful?
---
A successful team delivers,
and keeps delivering
---
## Delivering
<!-- .slide: data-background="./imgs/lucian-alexe-1MUBZt4zoJ0-unsplash.jpg" -->
---
Dealing with uncertainty
* sort by certainty <!-- .element: class="fragment" data-fragment-index="1" -->
* delay decisions <!-- .element: class="fragment" data-fragment-index="2" -->
* UI/UX before backend <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
accept that things are going to change

What are the right priorities

Reprioritise tasks in order of certainty.

Delay all decisions that can be delayed

Start with the frontend
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
* Knowledge sharing <!-- .element: class="fragment" data-fragment-index="3" -->
* Code reviews <!-- .element: class="fragment" data-fragment-index="4" -->

Note:
PRs with purpose (unsure, or needs validation, show and tell)

* push to master otherwise

* PR ARE A BLUNT TOOL FOR ENSURING CORRECTNESS
---
### Testing
* never postpone <!-- .element: class="fragment" data-fragment-index="1" -->
* the "acceptance test only" fallacy <!-- .element: class="fragment" data-fragment-index="2" -->
* dumb tests are fine <!-- .element: class="fragment" data-fragment-index="3" -->

Note:
Never postpone testing: test is supposed to help you, should not be a chore.
Automated tests should save your time. But the only do so if you don't postpone them.

If testing is difficult consider changing the code or changing testing strategy/level.

100% test coverage is often the wrong goal

try to cover 1 obvious cases and the corner cases
balance cost/convenience

Balance for acceptance and unit test:
"I don't need to write unit test because I am experienced enough to write modular/testable code. Also testing the implementation may become an hindrance when refactoring.
I only need to write acceptance test to ensure the correctness"
---
## keeps delivering
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
Tech debt
- only if necessary <!-- .element: class="fragment" data-fragment-index="1" -->
- documented <!-- .element: class="fragment" data-fragment-index="2" -->
- two types <!-- .element: class="fragment" data-fragment-index="3" -->
Note: 

There are 2 types of tech debt. The first one can be addressed the first time you change the code (as soon as it is documented clearly). I suggest to move this in the project board, to be picked up when you do any change to the the project.

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
- tech debt <!-- .element: class="fragment" data-fragment-index="5" -->

Note:
- document your love for the next dev. document why, tradeoffs, assumptions, tech debt
keep the documentation in the most obvious place and keep it up-to-date.
---
Microservice architecture principles:
- self containment <!-- .element: class="fragment" data-fragment-index="1" -->
- indipendence <!-- .element: class="fragment" data-fragment-index="2" -->

Note:
- a service FE should talk with its BE
- do not spread things across services
- fake endpoint to external services when practical
- create demo page
- fake the data (for test and demo)
---
Don't be too clever
- Keep it simple <!-- .element: class="fragment" data-fragment-index="1" -->
- "everybody does it" is no good reason <!-- .element: class="fragment" data-fragment-index="2" -->
- explicit is better than implicit <!-- .element: class="fragment" data-fragment-index="3" -->

Note: 
- Vanilla is better (keep things simple and do not use fancy libs, unless necessary or very convenient)
- do things for a reason
- use functional paradygm with moderation

- use rest sensibly, graphql is probably not the solution you are looking for
- redux-form
- do not use nesting on sass. Except for namespacing
- do not use fancy transpilation or macros

Use the minimal amount of things you need and do not over-engineer
---
Make a service observable:
- Monitoring, alerting <!-- .element: class="fragment" data-fragment-index="1" -->
- Audit <!-- .element: class="fragment" data-fragment-index="2" -->
- logs <!-- .element: class="fragment" data-fragment-index="3" -->

Note: 
dedicate time and attention on monitoring, alerting, audit, debugging helpers
---
## Solve a problem once
<!-- .slide: data-background="./imgs/view-ape-thinking-primate-33535.jpg" -->

---
## Be proud of what you achieve
<!-- .slide: data-background="./imgs/brown-primate-hanging-on-tree-1123771.jpg" -->
---
## Thanks
<!-- .slide: data-background="./imgs/black-chimpanzee-smiling-50582.jpg" -->
Let's keep in touch!
* @sithmel
* maurizio.lupo@gmail.com
