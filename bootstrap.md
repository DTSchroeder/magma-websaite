---
layout: page
title: Bootstrap
permalink: /bootstrap/
---

# Magma Bootstrap - Principled Construction

---

_NOTE: Uses Tractatus-style hierarchical numbering scheme to reflect the depth of each idea, making the logical flow and relationships between sections clear and easily navigable. The structure allows each principle or sub-principle to stand on its own, while still tying back to the larger concept._

---

### 1. Introduction

1.1 **Language shapes thought**: The way we model problems, reason about solutions, and compose systems is deeply influenced by the language we use.

1.2 **Program construction mirrors this principle**: Effective software development requires clear mental categories and conceptual foundations to guide modeling, reasoning, and abstraction.

1.3 **Magma is built on this principle**: The conceptual foundation of Magma aims to distill essential ideas about programming into a framework that transcends language or technology.

---

### 2. Conceptual Formation

2.1 **Conceptual clarity is key**: Just as language frames thought, in programming, clearly defined concepts structure our understanding of systems.

2.2 **Category Theory** provides a framework for composing abstract structures and relationships, offering deep insights into composition and behavior.

2.2.1 **Composability**: Complex systems can be constructed by composing simple, reusable parts.

2.2.2 **Abstract structures**: Category Theory enables reasoning about programs as abstract entities, removing the need for low-level details.

2.3 **Type Theory** focuses on ensuring correctness and composability through types.

2.3.1 **Correctness-by-construction**: Type theory ensures that systems are designed with correctness built into their foundations.

2.3.2 **Type-guided development**: The types used in a program guide the system’s composition and interaction.

2.4 **The mental toolkit for Magma** draws from these theoretical foundations.

2.4.1 **Minimal and systematic**: The toolkit is simple yet systematic, providing a foundation for creating reusable, flexible systems.

2.4.2 **Easy to learn**: The concepts in Magma are distilled to their essence, forming an easy-to-learn and powerful toolkit.

---

### 3. Transition to Type-Centric Construction

3.1 **Types are central to Magma’s philosophy**: Magma elevates types as the primary tool for designing and composing systems.

3.2 **The shift to a type-centric approach** ensures that types serve as the backbone for correctness, interaction, and decomposition of problems.

---

### 4. Principles of Type-Centric Construction

4.1 **Behavioral Type Abstraction**

4.1.1 **Defining interactions**: Behavioral Type Abstraction focuses on defining how system components interact.

4.1.1.1 **Interaction protocols**: These protocols are abstract contracts, defining how components communicate without binding them to specific implementations.

4.1.1.2 **Composability**: Behaviors are designed to be composed together, enabling the building of more complex interactions.

4.1.2 **Flexibility through decoupling**: By separating behavior from implementation, the system becomes more flexible and adaptable.

4.2 **Structural Type Composition**

4.2.1 **Composing systems from smaller pieces**: Structural Type Composition is about building complex systems by combining smaller, reusable types.

4.2.1.1 **Interface Composition**: Interfaces are incrementally combined to form cohesive, reusable systems.

4.2.1.2 **Separation of Concerns**: Each interface or type handles a specific aspect of the system, making it easier to reason about individual parts.

4.2.2 **Modularity and scalability**: The structure allows systems to grow organically, adding new features without altering existing systems.

4.3 **Arrangement of Type Structure**

4.3.1 **Logical organization of types**: Arrangement concerns the logical, hierarchical organization of types within the system.

4.3.1.1 **Hierarchical nesting**: Types are nested to reflect their logical relationships, ensuring modularity and navigability.

4.3.1.2 **Encapsulation and containment**: Nesting enforces scope and visibility, ensuring that components are appropriately isolated within the system.

4.3.2 **Clarity through naming and organization**: Clear, descriptive names and logical arrangement ensure that the system is easy to understand and navigate.

---

### 5. Orthogonal Complementary Principles

5.1 **Behavioral Type Abstraction, Structural Type Composition, and Arrangement of Type Structure are orthogonal principles**.

5.1.1 **Behavioral Type Abstraction**: Defines protocols and composable behaviors, independent of system composition.

5.1.2 **Structural Type Composition**: Focuses on assembling systems from modular components.

5.1.3 **Arrangement of Type Structure**: Governs the organization and placement of types within the system.

5.2 **These principles complement each other**: When combined, they form a cohesive strategy for building maintainable, scalable, and flexible systems.

5.2.1 **Flexibility**: Optional behaviors allow systems to be dynamically reconfigured without altering their core structure.

5.2.2 **Modularity**: Structural composition and arrangement enhance the modularity of the system.

5.2.3 **Navigability**: Logical arrangement ensures that even complex systems remain understandable.

5.3 **Arrangement Enhances Abstraction and Composition**

5.3.1 **Nesting and encapsulation**: The arrangement of types reflects their abstract relationships and enforces encapsulation.

5.3.2 **Semantic clarity**: Proper arrangement ensures that types and their roles within the system are clear.

5.4 **Incremental construction through arrangement**: The logical layering of types facilitates composition and reuse.

5.5 **Conclusion: Integrating the Principles**

5.5.1 By applying Behavioral Type Abstraction, Structural Type Composition, and Arrangement of Type Structure, Magma enables the creation of modular, scalable, and maintainable systems.

5.5.2 **The power of type-centric construction**: This approach emphasizes clarity, flexibility, and correctness, resulting in systems that can evolve over time while maintaining structural integrity.

---

### 6. Departure from Classical Object-Oriented Programming

6.1 **A shift from class inheritance to behavior composition**:

6.1.1 **Classical OOP relies on inheritance**, which can lead to tightly coupled, rigid systems.

6.1.2 **Type-Centric Construction focuses on behavior composition**, allowing flexible and dynamic system construction.

6.2 **Modularity and reusability**:

6.2.1 **Classical OOP suffers from deep inheritance chains**, which can limit reusability and clarity.

6.2.2 **Type-Centric Construction breaks functionality into composable units**, improving modularity and reuse.

6.3 **Abstraction of types and interactions**:

6.3.1 **Classical OOP couples data with behavior**, leading to tight coupling between objects.

6.3.2 **Type-Centric Construction abstracts types by their interactions**, ensuring components remain loosely coupled and adaptable.

---

### 7. Rising to Higher-Order

7.1 **Beyond methods and objects**: Magma moves beyond the confines of methods tied to objects, embracing the power of higher-order abstractions.

7.2 **Higher-Order Concept**: In general, “higher-order” refers to abstractions that operate on other abstractions. This means that higher-order entities can take other entities as input or produce them as output.

7.3 **Functions as First-Class Citizens**: Treat functions with the same importance as objects, allowing them to be passed as arguments, returned from other functions, and stored in variables. This unlocks powerful functional programming patterns.

7.4 **Higher-Order Functions**: `Fn0`, `Fn1`, ... `Fn8` represent function types that take zero to eight arguments respectively.

7.5 **Inductive Construction of Function Types**

    ```
    interface Fn1<A, B>
    interface Fn2<A, B, C> extends Fn1<A, Fn1<B, C>>
    interface Fn3<A, B, C, D> extends Fn2<A, B, Fn1<C, D>>
    interface Fn4<A, B, C, D, E> extends Fn3<A, B, C, Fn1<D, E>>
    interface Fn5<A, B, C, D, E, F> extends Fn4<A, B, C, D, Fn1<E, F>>
    interface Fn6<A, B, C, D, E, F, G> extends Fn5<A, B, C, D, E, Fn1<F, G>>
    interface Fn7<A, B, C, D, E, F, G, H> extends Fn6<A, B, C, D, E, F, Fn1<G, H>>
    interface Fn8<A, B, C, D, E, F, G, H, I> extends Fn7<A, B, C, D, E, F, G, Fn1<H, I>>
    ```

7.5.1 **Currying**: Decomposition of multi-argument functions into nested single-argument functions, facilitating deferred execution.

7.5.2 **Partial Application**: Creation of specialized functions by pre-setting some arguments of a more general function.

7.6 **Benefits of Magma's Approach**:

- **Enhanced Modularity**: Functions become reusable building blocks, fostering cleaner and more maintainable code.

- **Increased Expressiveness**: Higher-order functions and currying provide a richer vocabulary for expressing computations.

- **Deferred Execution**: Currying enables you to delay the execution of a function until all arguments are available.

- **Code Adaptability**: Partial function application creates specialized functions from more general ones, promoting code reuse.

7.7 **Conclusion**

Magma empowers you to write code that is more modular, expressive, and adaptable by embracing higher-order functions and inductive function type construction. This functional programming approach unlocks new possibilities for building elegant and efficient software systems.

### 8. Functorial Abstractions

8.1 **Beyond Higher-Order Functions**: Magma extends its conceptual framework further by incorporating functorial abstractions, which are central to functional programming and provide powerful tools for composing computations and transformations.

8.2 **Higher-kinded Type Approximation**:

- Java lacks native support for higher-kinded types.
- The design uses a recursive type parameter {@code U} to approximate higher-kinded types, effectively encoded as a type-level defunctionalized representation.
- The recursive bounded unification parameter {@code U} expresses type relationships that are enforced at compile-time, ensuring strong type safety for all functor operations.
- Modeling Parametric Type Relationships:
  - {@code A}: Functor’s carrier parameter
  - {@code U}: Unification parameter representing the functor type
  - {@code U extends Functor<?, U>}: Recursive bound that ensures the functor is related to itself
- Enforcing Parametric Compile-time Type Constraints
  - Any type used as {@code U} must implement the {@code Functor} interface
  - Operations using {@code U} guarantee the presence of functorial behaviors
  - Operations returning {@code U} allow for type-safe, covariant subtype flexibility

8.3 **Functor**:

- **Covariant Transformations**: Represents types that can be mapped over, preserving their structure.
- **Functor Operations**:
  - **`map`**: Lifts a pure function `A -> B` into the functor's context, transforming a `Functor<A>` into a `Functor<B>`.
- **Functor Laws**:
  - **Composition**: `fa.map(f).map(g) ≡ fa.map(f.then(g))`
  - **Identity**: `fa.map(x -> x) ≡ fa`
- https://gist.github.com/TobiasHerb/18c7ee4ed13319371ee45d873c6212e8

8.4 **Contravariant**:

- **Contravariant Transformations**: Represents types that can be contra-mapped over (transformations in the opposite direction of a functor).
- **Contravariant Operations**:
  - **`contramap`**: Maps a function `B -> A` over the contravariant functor, changing its carrier type from `A` to `B`.
- **Contravariant Functor Laws**:
  - **Composition**: `fa.contramap(f).contramap(g) ≡ fa.contramap(g.andThen(f))`
  - **Identity**: `fa.contramap(x -> x) ≡ fa`
- https://gist.github.com/TobiasHerb/845db16cec728b7cad08e8b45ff3f0ae

8.5 **Bifunctors**:

- **Transformations on Two Types**: Represents types that carry two values and allow transformations on both simultaneously.
- **Bifunctor Operations**:
  - **`bimap`**: Takes two functions, one for each carrier type, and applies them concurrently.
  - **`bimapL`**:
  - **`bimapR`**:
- **Bifunctor Laws**:
  - **Composition**: `fa.bimap(f, g).bimap(h, i) ≡ fa.bimap(f.then(h), g.then(i))`
  - **Identity**: `fa.bimap(x -> x, y -> y) ≡ fa`
- https://gist.github.com/TobiasHerb/e99d246487727adf94d3ded0d6f378bb

8.6 **Profunctors**:

- **Generalization of Functions**: Combine contravariant and covariant transformations.
- **Profunctor Operations**:
  - **`dimap`**: takes a contravariant function for the input type and a covariant function for the output type.
- **Profunctor Laws**:
  - **Composition**: `pf.dimap(f, g).dimap(h, i) ≡ pf.dimap(f.then(h), g.then(i))`
  - **Identity**: `pf.dimap(x -> x, y -> y) ≡ pf`
- **Specialized Profunctor types**:
  - **Cartesian**:   Represent profunctors that work with Cartesian product types, facilitating operations on pairs of values.
  - **Cocartesian**: Represent profunctors that work with coproduct (sum) types, enabling operations on values that can be one of two types.
- https://gist.github.com/TobiasHerb/96861710983bfed8e6cdc4b8286b7fd5
- https://gist.github.com/TobiasHerb/7df474f361aa2c6f2868db45e161f54c
- https://gist.github.com/TobiasHerb/a4e6daa38a2aa6576b88685101498ec0

8.7 **Applicatives**:

- **Extension of Functors**: Applicatives extend the capabilities of functors by providing a way to apply functions within a context to values within another context.
- **Applicative Operations**:
  - **`pure`**: Lifts a pure value into the applicative context.
  - **`zap`**: Applies a function wrapped in an applicative to a value wrapped in another applicative.
- **Applicative Laws**:
  - **Identity**: `fa.zap(pure(id())) ≡ fa`
  - **Homomorphism**: `pure(f).zap(pure(x)) ≡ pure(f(x))`
  - **Interchange**: `ff.zap(pure(x)) ≡ pure(f -> f(x)).zap(ff)`
  - **Composition**: `pure(compose).zap(f).zap(g).zap(h) ≡ f.zap(g.zap(h))`
- https://gist.github.com/TobiasHerb/070b07976f6cbfcdee77c46b9e60e19e
- https://gist.github.com/TobiasHerb/f253f26eb51c1d50aaffa31675fdf966

8.8 **Monads**:

- **Extension of Applicatives**: Monads build upon applicatives by introducing the ability to flatten nested structures. This is crucial for handling computations that may produce other computations as their results.
- **Monad Operations**:
  - **`flatmap`**: Takes a function that returns a monad and applies it to the current monad's value, then flattens the resulting nested monad.
- **Monad Laws**:
  - **Left Identity**: `pure(a).flatmap(f) ≡ f.apply(a)`
  - **Right Identity**: `ma.flatmap(pure) ≡ ma`
  - **Associativity**: `ma.flatmap(f).flatmap(g) ≡ ma.flatmap(a -> f.apply(a).flatmap(g))`
- **Specialized Monad types**:
  - `Reader`:  Models computations that depend on an environment.
  - `Writer`:  Models computations that produce a value along with a log or side effect.
  - `Error`:   Models computations that can either succeed with a value or fail with an error.
- https://gist.github.com/TobiasHerb/876aa48cf9801118af49fcb78456b3a3

8.9 **Benefits of Functorial Abstractions**:

- **Compositionality**: Functors, and their extensions, enable the creation of complex transformations by composing simpler ones.
- **Abstraction**: They provide a way to abstract over common patterns of computation and data transformation.
- **Type Safety**: The use of type parameters and bounds ensures that operations are type-safe, preventing errors at compile time.
- **Expressiveness**: They allow for concise and elegant expression of computations that involve effects, context, or complex data structures.

8.8 **Conclusion**:

Magma's incorporation of functorial abstractions provides a powerful toolkit for structuring and composing computations in a type-safe and principled manner. These abstractions, combined with the focus on higher-order functions and type-centric construction, enable developers to build modular, reusable, and maintainable software systems that are adaptable to changing requirements and complexities.

---

## APPENDIX

### ANALYSIS: Type-Centric Construction of Magma’s Algebraic Data Types (ADTs)
In this detailed case study of **Magma’s Algebraic Data Types (ADTs)**, we will analyze how the **Principles of Type-Centric Construction** — **Behavioral Type Abstraction**, **Structural Type Composition**, and **Arrangement of Type Structure** — are applied to the structure and behavior of products, coproducts, and slots within the framework. The key concepts, such as **slot projections**, **compound projections**, **injections**, and **pattern matching**, exemplify these principles in a cohesive and scalable manner.

- **Overview**
  - https://gist.github.com/TobiasHerb/8ee7a24beab3ccce72612a67f930e177
  - https://gist.github.com/TobiasHerb/b6f25be5f67b518df67b838104f00d50
  - https://gist.github.com/TobiasHerb/3fb43af7e5ceeff7c7f7deaa6a156ce1
  - https://gist.github.com/TobiasHerb/286a978491eb681b2b8b9b01aa91a6f6 
  - **Magma’s Algebraic Data Types (ADTs)** are analyzed through the lens of the **Principles of Type-Centric Construction**.
    - **Behavioral Type Abstraction**
    - **Structural Type Composition**
    - **Arrangement of Type Structure**
  - Key concepts:
    - **Slot projections**
    - **Compound projections**
    - **Injections**
    - **Pattern matching**
- **Behavioral Type Abstraction in Magma’s ADTs**
  - **Defining Interactions**
    - Interfaces like `Slot`, `Compound`, and `Product` define **interaction protocols**.
    - **Slot interface**:
      - Example: `non-sealed interface $_1<A> extends Slot { A _1(); }` 
      - Behavior: Accessing the first component of a compound type.
    - **Compound projection**:
      - Example:`non-sealed interface Of2<A, B> extends Compound, Of1<A>, Slot.$_2<B> { }`
      - Behavior: Interacting with multiple slots.
  - **Flexibility through Decoupling**
    - **Decoupling interactions from implementations** allows customized behavior without affecting other types.
    - Example:`non-sealed interface $_1<A, R> extends Slot.In<R> { R _1(A a); }`
      - The behavior of projection and injection can be composed, as in `Product3<A, B, C>`.
- **Structural Type Composition in Magma’s ADTs**
  - **Composing Systems from Smaller Pieces**
    - Magma’s ADT structure is composed incrementally from simpler types.
    - **Product2**: `non-sealed interface Product2<A, B> extends Product1<A>, Compound.Of2<A, B> { B _2(); }`
    - **Product3**: `non-sealed interface Product3<A, B, C> extends Product2<A, B>, Compound.Of3<A, B, C> { C _3(); }`
  - **Modularity and Scalability**
    - **Product** and **Coproduct** types promote modularity and scalability.
    - **Coproduct2** example:`public non-sealed interface Coproduct2<A, B> extends Coproduct { <R> R match(Fn1<? super A, ? extends R> case1, Fn1<? super B, ? extends R> case2); }`
    - Composition is extended in `Coproduct3<A, B, C>`.
- **Arrangement of Type Structure in Magma’s ADTs**
  - **Logical Organization of Types**
    - Types are **logically nested** and hierarchically arranged.
    - Example:`non-sealed interface $_1<A> extends Slot { A _1(); }`
  - **Clarity through Naming and Organization**
    - Naming conventions provide **semantic clarity**.
    - Example:
      - `Product3<A, B, C>` indicates a product type with three components.
      - **Compound types** (e.g., `Compound.In.To3<A, B, C, R>`) are similarly clear.
- **Orthogonal Complementary Principles in Magma’s ADTs**
  - **Orthogonality**
    - Each principle operates independently:
      - **Behavioral Type Abstraction**: Encapsulates component interaction.
      - **Structural Type Composition**: Composes interactions to form complex structures.
      - **Arrangement of Type Structure**: Ensures logical organization of types.
  - **Complementarity**
    - The principles ensure flexibility, modularity, and navigability.
    - Slot projections and compound types provide modularity, while type arrangement ensures clarity.
- **Conclusion**
  - The **Principles of Type-Centric Construction** (Behavioral Type Abstraction, Structural Type Composition, Arrangement of Type Structure) create a **modular, scalable, and flexible** system in Magma’s ADTs.
    - Focus: Interaction protocols, reusable type compositions, clear organizational hierarchies.
    - Outcome: Ease of understanding, extension, and maintenance of complex types like **Products** and **Coproducts**.