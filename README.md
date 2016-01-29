# SOLID Thinking

## Start Here

[Solid Principles in Ruby][1]
November 29, 2013
Well written with clear examples of each principle. I think I like this one better than the Back to Basics article.

> This one is simpler to demonstrate, if you have a class that has two clients (objects using it):

I like this. It seems to be a simple statement, but takes the time to define the word 'clients'.

[Back to Basics: SOLID][2]
September 03, 2014
An introduction to the SOLID principles with some basic examples.

#### Questions

> It’s also not uncommon to see methods overridden with modified method signatures causing branching on type in classes that depend on objects of the parent’s type.

I don't understand the words that are coming out of your mouth.

> The Dependency Inversion Principle has to do with high-level (think business logic) objects not depending on low-level (think database querying and IO) implementation details.

It would be nice to see the example re-written to violate the principle.

## Let's Make Headway

Given these descriptions, can we rewrite them using even more layman's terms or at least our own terms?

---

#### SRP - Single responsibility principle

A class should have only a single responsibility.

Every class should have a single responsibility, and that responsibility should be entirely encapsulated.
All its services should be narrowly aligned with that responsibility, this embrace the high cohesion.

---

#### OCP - Open/closed principle

Software entities should be open for extension, but closed for modification.

That is, such an entity can allow its behaviour to be extended without modifying its source code.

---

#### LSP - Liskov substitution principle

Objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program.

It states that, in a computer program, if S is a subtype of T, then objects of type T may be replaced with objects of type S (i.e., objects of type S may substitute objects of type T) without altering any of the desirable properties of that program (correctness, task performed, etc.)

---

#### ISP - Interface segregation principle

Many client-specific interfaces are better than one general-purpose interface.

States that no client should be forced to depend on methods it does not use.

ISP splits interfaces which are very large into smaller and more specific ones so that clients will only have to know about the methods that are of interest to them. Such shrunken interfaces are also called role interfaces.

ISP is intended to keep a system decoupled and thus easier to refactor, change, and redeploy.

---

#### DIP - Dependency inversion principle

One should Depend upon Abstractions, Do not depend upon concretions.

Refers to a specific form of decoupling software modules. When following this principle, the conventional dependency relationships established from high-level, policy-setting modules to low-level, dependency modules are inverted (i.e. reversed), thus rendering high-level modules independent of the low-level module implementation details.

---

[1]: https://subvisual.co/blog/posts/19-solid-principles-in-ruby
[2]: https://robots.thoughtbot.com/back-to-basics-solid
