# Importance of Software Architecture and Principles of Great Design

It will focus on the key aspects to keep in mind when designing the architecture of a C++ solution.

## Understanding software architecture

- When you write some codes or project , you have to deal with which component interact with others. When desinging the architecture you have to think big picture. 
  
- On a small scale , every single building looks okay , but they dont combine into sensible  bigger picture.
  
- The software architecture of a system is the set of structures needed to
reason about the system, which comprise software elements, relations
among them, and properties of both.

- Enterprise architecture deals with the whole company or even a group of companies. When thinking about enterprise architecture, ypu should be looking at how all the systems in company behave and cooperate with each other. Its concerned about the alignment between business and IT
- Solution architecture is less abstract than its enterprise counterpart.Usually, solution architecture is concerned with one specific system and the way it interacts with its surroundings. 
- Software arhitecture is even more concrete than solution architecture. It concentrates on a specific project , the technologies it uses and how it interacts with other projects.
- Infrasturucture architecture is , as the name suggests, concerned about the infrasture that software will use. It defines the deployment environment and strategy,how the application will scale , fail handling , site reliability and other.

## Learning the importance of proper architecture

If after several months or even years of development you still want your software to retain its qualities, you need to take some steps earlier in the process.

### Software decay

Software decay, sometimes also
called erosion, occurs when the implementation decisions don't correspond
to the planned architecture. All such differences should be treated as
technical debt.

### Accidental Arhitecture

Generally speaking, if your
software is getting tightly coupled, perhaps with circular dependencies, but
wasn't like that in the first place, it's an important signal to put more
conscious effort into how the architecture looks


### Exploring the fundamentals of good architecture

- Architecture context
- Stakeholders
- Business and technical environments

### Developing architecture using Agile principles

Agile , by nature , is iterative and incremental.

- Managing architecture doesnt need to mean keeping massive documentation.In fact, It sould be simple and cover only relevant views of the system.
  
### Domain-driven Design

Domain-driven design , or DDD for short. a major software design approach, focusing on modeling software to match a domain according to input from that domain's experts.
DDD ilk olarak Eric Evans tarafından ortaya atılmış ve bir çok konuda olduğu gibi Martin Fowler’dan da destek görmüş bir yaklaşımdır. Eric Evans büyük ve karmaşık sistemlerdeki sorunların domainlere bölünerek, kendi domaini içerisinde çözülmesi gerektiğini savunmaktadır. Bu problemlerin çoğunun business taraf ile teknik tarafın ortak bir dil konuşamamasından ve yazılımın doğru modellenmemesinden kaynaklı olduğunu düşünmektedir.

Her yazılımın kendine has olayları ve ilgi alanları vardır.

### The philosophy of C++
Using higher-level abstractions leads to simpler, more maintainable code.
The C++ language has strived to provide zero-cost abstractions since its
inception, so build upon that instead of redesigning the wheel using lower
levels of abstraction.

### Following the SOLID and DRY principles
- Single responsibility principle
- Open-closed principle
- Liskov substitution principle
- Interface segregation
- Dependency Inversion


Some of the examples use dynamic polymorphism, but the same would
apply to static polymorphism. If you're writing performance-oriented code
(and you probably are if you chose C++), you should know that using
dynamic polymorphism can be a bad idea in terms of performance,
especially on the hot path. Further on in the book, you'll learn how to write
statically polymorphic classes using the Curiously Recurring Template
Pattern (CRTP).

#### Single Responsibility Principle

- Each code unit should have exactly one responsibility.


#### Open-closed Principle

- “When a single change to a program results in a cascade of changes to dependent modules, that program exhibits the undesirable attributes that we have come to associate with ‘bad’ design. The program becomes fragile, rigid, unpredictable and unreusable. The open-closed principle attacks this in a very straightforward way. It says that you should design modules that never change. When requirements change, you extend the behaviour of such modules by adding new code, not by changing old code that already works.”


#### Liskov Substitution Principle



## Reference
1.<https://www.linkedin.com/pulse/software-entropy-continuous-state-decay-dennis-van-wattingen/>
2.<https://medium.com/kariyertech/domain-driven-design-643c02168ecc>
3.<https://www.gencayyildiz.com/blog/domain-driven-design-stratejik-ve-taktiksel-olarak-derinlemesine-inceleme/>
4.<https://www.vishalchovatiya.com/open-closed-principle-in-cpp-solid-as-a-rock/>
5.<https://www.softwareyoga.com/open-closed-principle/>
6.<https://medium.com/@emreozguruoglu/the-liskov-substitution-principle-lsp-liskovun-yerine-geçme-prensibi-nedir-70b5daa4d8b9>