---
layout: toc_page
title: PRINCIPLES OF PROGRAM CONSTRUCTION
permalink: /princples/
---

(focus: interface type abstraction)

---

## **I. ABSTRACTION OF TYPE STRUCTURE**

**Abstraction of Structure** refers to the **conceptual encapsulation** of behavior and properties within **interface types**, providing a generalized and flexible mechanism for interaction. 

Concerned with encapsulation by hiding specifics behind a **uniform interface**, thus promoting flexibility, reusability, and decoupling between components.

- **Interface Type Abstraction**: Interfaces define a **contract** that abstracts the underlying implementation. By specifying operations without detailing how they are performed, interfaces allow for **polymorphic behavior** where multiple implementations can conform to the same structural interface. 
- **Parametric Abstraction**: Through **type parameters** and **type bounds**, abstractions are extended to work over multiple types, ensuring that operations remain generic and flexible while being type-safe.
- **Behavioral Abstraction**: Abstraction in interfaces also extends to **protocols of interaction**, where behavior can be defined but not tied to a particular implementation, promoting reuse in various contexts.
- **Role in Type Structure**: Abstraction allows us to create a **hierarchy** of concepts that are disconnected from implementation details, making it easier to model complex systems by focusing on essential behaviors and relationships.

**Key Principles**:
- Abstraction hides complexity while exposing necessary behaviors.
- Interfaces serve as the backbone of abstraction, supporting a modular and extensible type system.
- It promotes decoupling and flexibility by defining **contracts** that can be realized through multiple implementations.

---

## **II. COMPOSITION OF TYPE STRUCTURE**

Emphasizes the **modular construction** of types, particularly through **mixin interfaces** and **inheritance mechanisms**. 

Concerned with how multiple types, particularly interfaces, are composed to form **new structures**.

- **Interface Composition**: Here, interfaces are **composed incrementally** using mixins, combining simpler abstractions into more complex types. This allows for modular development, where each type or interface can be composed from smaller, well-defined parts.
- **Separation of Concerns**: Composition allows for a clear **separation of concerns**, where each interface handles a specific aspect or concern, and these concerns are combined to form a holistic structure.
- **Hierarchical and Scalable**: Composition supports the **incremental construction** of types, where each interface layer builds upon previous ones, forming a **hierarchical system**. This ensures scalability and flexibility in the way types are organized and extended.
- **Role in Type Structure**: Composition focuses on **how** types are built and combined, promoting **reuse** of common functionality and enabling **scalable** and **manageable** structures through incremental type layering.

**Key Principles**:
- Composition promotes **reuse** and modularity by constructing types from smaller, composable units.
- Mixins and inheritance mechanisms are key to forming complex types from simpler building blocks.
- The focus is on **how** types are put together to build more complex systems.

---
## **III. ARRANGEMENT OF TYPE STRUCTURE**

Emphasizes the **logical organization** and **structural layout** of types, ensuring that systems are **modular**, **navigable**, and **scalable**. It governs how types, particularly interfaces, are nested and named, reinforcing clear containment, encapsulation, and semantic coherence.

Concerned with the organization of types in a way that reflects their **logical relationships**, supports **modularity**, and enhances **readability and maintainability**.

- **Hierarchical Composition**: Types are arranged in **nested hierarchies**, reflecting the natural **correspondence between types and their roles** within the system. This organization ensures that relationships between types are intuitive and maintainable, creating a logical hierarchy that scales with complexity.
- **Encapsulation**: Nested structures **enforce scope and visibility**, ensuring that internal components are **encapsulated** within their aggregates. This promotes strong **part-whole relationships**, where components are accessible only within the proper context, enhancing modularity.
- **Containment**: Nested types clearly **model logical containment**, with each type placed within the structure that it supports. This preserves the **logical relationships** between higher-level abstractions and their contained components.
- **Namespace Management**: By **nesting type declarations**, the system defines clear **namespace boundaries**, avoiding naming conflicts and maintaining a meaningful **contextual namespace**. This arrangement prevents ambiguity and fosters readability.
- **Lexical Polymorphism**: Nested types allow for **name reuse** within their context, avoiding naming conflicts while retaining **qualified names** that reflect their purpose. This supports flexibility and avoids redundancy in naming, while maintaining clear context.
- **Semantic Clarity in Naming**: Type names reflect their **roles and positions** within the structure, providing a natural mapping between **names and purposes**. This ensures that the structure remains intuitive and easy to navigate, with names clearly indicating their functions within the hierarchy.
- **Role in Type Structure**: The **arrangement of structure** focuses on how types, especially interfaces, are **positioned and related**, ensuring that the system remains **scalable**, **navigable**, and **semantically coherent**. Proper arrangement helps maintain clarity and context as the system grows in complexity.

**Key Principles**:
- Arrangement ensures a clear **hierarchical organization** that mirrors the logical relationships between types.
- It promotes **modularity and encapsulation** through nested structures that define proper scoping and containment.
- Proper namespace management and **qualified naming** prevent naming conflicts and enhance the clarity of type roles. 

---

## ORTHOGONAL COMPLEMENTARY PRINCIPLES

Abstraction, composition, and arrangement of type Structure are to be considered as **orthogonal principles**. Each of these principles addresses **distinct and independent aspects** of how types are structured, organized, and interact, particularly with a focus on **interface type abstraction**. While they contribute to the overall coherence and modularity of a system, they operate in different dimensions, providing separate yet complementary benefits to type organization.

- **Abstraction of Type Structure**
  - Focuses on the **conceptual encapsulation** of behavior and properties within **interface types**. It separates the **what** from the **how**, ensuring that interfaces represent generalized contracts that **abstract implementation details**. The principle of abstraction is concerned with **hiding complexity** while exposing necessary behaviors, allowing for **polymorphic and flexible** system design.
  - Orthogonal Role: Abstraction deals with **decoupling** and **hiding implementation specifics**, which is distinct from how types are combined (composition) or organized (arrangement). It governs the level of generalization and flexibility within a system by providing **uniform interfaces** for interaction.
- **Composition of Type Structure**
  - Emphasizes the **modular construction** of types, particularly through **mixins** and **inheritance**. It is concerned with **how types are built** from smaller, reusable components. The goal is to form new, complex types by **combining simpler abstractions** in an incremental, layered manner, allowing for the **reuse of common functionality**.
  - Orthogonal Role: Composition focuses on the **construction and layering of types**, independent of how these types are abstracted or arranged. Its primary concern is with **modularity and reusability**, ensuring that systems can scale through **type composition**.
- **Arrangement of Type Structure**
  - Addresses the **logical organization** of types, ensuring that the system is **navigable**, **modular**, and **scalable**. It governs how types are **nested**, **named**, and **scoped**, ensuring that their relationships are clear and their purpose within the system is semantically meaningful. The principle of arrangement ensures that **logical hierarchies** and **containment** relationships are properly maintained.
  - Orthogonal Role: Arrangement deals with the **positioning** and **organization** of types within the system. It operates independently of how the types are abstracted (abstraction) or composed (composition), focusing instead on how to make the system **semantically coherent** and **structurally navigable**.

**Orthogonal Interaction**

These principles are orthogonal because they represent different facets of type structure, and they do not overlap in their concerns:

- **Abstraction** is about **hiding complexity** and **defining contracts** through interface types.
- **Composition** is about **building types** through **reusable components** and **mixins**.
- **Arrangement** is about **organizing types** in a **logical hierarchy** that reflects **containment** and **encapsulation**.

Although orthogonal, these principles complement each other, ensuring that a well-designed system is **flexible**, **modular**, and **navigable**:

- **Abstraction** enables **flexibility and polymorphism** by abstracting away implementation specifics.
- **Composition** ensures that the system can **scale and be reused** through **modular construction**.
- **Arrangement** guarantees that the system remains **clear and navigable**, with types **organized** in a way that reflects their roles and relationships.

---

## ARRANGEMENT BUILDS UPON ABSTRACTION/COMPOSITION

**Arrangement** of type structure builds upon both **Abstraction** and **Composition** by establishing clear **hierarchical organization**, **visibility rules**, and **semantic clarity** for how types, especially interfaces, are arranged within a system. It focuses on ensuring that the type structures, once abstracted and composed, are logically organized and navigable. This aspect addresses how the types are **logically laid out** to form a coherent, scalable, and semantically meaningful system.

**RELATIONSHIP WITH ABSTRACTION**
- **Hierarchical Composition** and **Containment**: When interfaces abstract behavior, their nesting reflects the **hierarchical relationships** between abstractions. The arrangement ensures that higher-level interfaces encapsulate general behavior, while more specific interfaces or implementations are nested within, **inheriting and refining the abstraction**. This nesting enforces clear containment, where **general abstractions** contain **specific realizations**.
- **Encapsulation and Namespace Management**: Abstracted types often need **explicit scoping** to maintain clarity. By nesting interfaces, you reinforce the **scope of access**, ensuring that abstract behavior is **encapsulated** and accessible only where necessary. This prevents implementation leakage, ensuring that abstract behavior remains appropriately confined, enhancing **namespace management** and **encapsulation**.
- **Lexical Polymorphism and Semantic Clarity**: The **names** used within nested structures carry clear, contextual meanings tied to their **abstract roles**. By embedding interfaces and types hierarchically, the system reflects **natural semantic relationships** between abstract concepts, reinforcing both **polymorphic reusability** and **clear naming conventions**.

**RELATIONSHIP WITH COMPOSITION**
- **Hierarchical Composition**: Composition is enhanced by **logical arrangement**. Nested structures enable **incremental and layered construction**, where composable components like mixins can be **contained and arranged** logically. This hierarchical approach mirrors the compositional process by making it clear how types build on one another, creating **layered, reusable constructs**.
- **Encapsulation and Containment**: As types are **composed**, especially via mixins and inheritance, arranging them in nested structures ensures that the **component parts remain encapsulated** within their composed whole. This guarantees that each composable unit operates within its intended scope, preserving **containment relationships** and **modular boundaries**.
- **Namespace Management and Qualified Naming**: When composing structures, proper **namespace management** prevents naming conflicts across complex systems. By organizing types and interfaces into **qualified, nested namespaces**, composed structures remain contextually clear and navigable. This helps maintain the integrity of composed types without risking **ambiguity** or **name collisions**.
- **Semantic Clarity in Naming**: As interfaces and types are composed, their names should reflect their roles within the larger system. Proper arrangement ensures that **type names convey purpose**, allowing developers to understand their **composed role** within the overall system, aligning with the goals of compositional hierarchy.

The arrangement of type structure provides the **logical scaffolding** necessary for managing both **abstraction** and **composition**. It ensures that abstract concepts and composable units are arranged in a way that promotes **modularity**, **encapsulation**, **clarity**, and **scalability**. By leveraging hierarchical composition, containment, and namespace management, the system becomes **navigable** and **semantically coherent**, ensuring that both abstracted and composed types function cohesively within the overall type structure.

---

## JAVA LANGUAGE-LEVEL MECHANISMS OF POLYMORPHISM

- **Subtype Polymorphism**
    - Inclusion Polymorphism (Orthogonal Mixin Interfaces)
    - Restricting Polymorphism (Sealed Interfaces)
    - Intersection Types (Multiple Interface Implementation)

- **Parametric Polymorphism (Generics)**
    - Bounded Parametric Polymorphism (Bounded Generics)
    - Wildcard Polymorphism (Unbounded Generics)

- **Behavioral Polymorphism**
    - Lambda Expressions and Functional Interfaces
    - Structural Polymorphism (Default Methods)
    - Signature (Ad-hoc) Polymorphism (Method Overloading)
    - Covariant Return Types (Overriding)

**TODO: Assign => Abstraction, Composition, Arrangement**

---

## CONCLUSION

By applying these principles in parallel, a system can achieve **conceptual clarity**, **modular extensibility**, and **logical coherence**, ensuring that it is both **maintainable** and **scalable**.

----

## EXAMPLE: TRAVERSAL SYSTEM

```java 
/**
 * Base abstraction for traversal operators.
 *
 * @param <F> type of 2nd-order traversal action
 */
public sealed interface TraverSystem<F> {
    
    /**
     * Step-based traversal operators.
     *
     * @param <F> type of 2nd-order traversal action
     */
    sealed interface Step<F> extends TraverSystem<F> {
        
        /**
         * Single-step traversal in the forward direction.
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Next<F> extends TraverSystem.Step<F> {
            /**
             * Performs a single forward step with the given action.
             *
             * @param action the action to apply during traversal
             * @return true if the action was applied, false if traversal is exhausted
             */
            boolean next(F action);
        }
        
        /**
         * Single-step traversal in the backward direction.
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Prev<F> extends TraverSystem.Step<F> {
            /**
             * Performs a single backward step with the given action.
             *
             * @param action the action to apply during traversal
             * @return true if the action was applied, false if traversal is exhausted
             */
            boolean prev(F action);
        }
    }
    
    /**
     * Bulk traversal operators.
     *
     * @param <F> type of 2nd-order traversal action
     */
    sealed interface For<F> extends TraverSystem<F> {
        
        /**
         * Bulk traversal in the forward direction.
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Next<F> extends TraverSystem.For<F> {
            /**
             * Applies the given action to all remaining forward steps.
             *
             * @param action the action to apply during traversal
             */
            void forNext(F action);
        }

        /**
         * Bulk traversal in the backward direction.
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Prev<F> extends TraverSystem.For<F> {
            /**
             * Applies the given action to all remaining backward steps.
             *
             * @param action the action to apply during traversal
             */
            void forPrev(F action);
        }
    }
    
    /**
     * Continuation-controlled bulk traversal operators.
     *
     * @param <F> type of 2nd-order traversal action
     */
    sealed interface While<F> extends TraverSystem<F> {
        
        /**
         * Continuation-controlled forward traversal.
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Next<F> extends TraverSystem.While<F> {
            
            /**
             * Applies the given action while the continuation predicate is satisfied.
             *
             * @param until the condition to stop traversal
             * @param <C> the type of control flow used during traversal
             * @return a predicate to control traversal
             */
            <C extends Eval.Control> Fn1.Predicate<C> whileNext(Fn1<C, F> until);

            /**
             * Applies the given action continuously.
             *
             * @param action the action to apply
             * @param <C> the type of control flow used during traversal
             * @return a predicate to control traversal
             */
            default <C extends Eval.Control> Fn1.Predicate<C> whileNext(F action) {
                return whileNext(Fn.constantly(action));
            }
        }
        
        /**
         * Continuation-controlled backward traversal.
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Prev<F> extends TraverSystem.While<F> {
            
            /**
             * Applies the given action while the continuation predicate is satisfied in reverse.
             *
             * @param until the condition to stop traversal
             * @param <C> the type of control flow used during traversal
             * @return a predicate to control traversal
             */
            <C extends Eval.Control> Fn1.Predicate<C> whilePrev(Fn1<C, F> until);

            /**
             * Applies the given action continuously in reverse.
             *
             * @param action the action to apply
             * @param <C> the type of control flow used during traversal
             * @return a predicate to control traversal
             */
            default <C extends Eval.Control> Fn1.Predicate<C> whilePrev(F action) {
                return whilePrev(Fn.constantly(action));
            }
        }
    }
    
    /**
     * A traverser to pass through an source of values in a unidirectional fashion.
     *
     * <p>The following traversal operators are available:
     * <ul>
     *   <li>{@code #next(Fn1.Action)}: Single-step TraverSystem.
     *   Each remaining value is traversed one-by-one, via repeated invocations.
     *
     *   <li>{@code #forNext(Fn1.Action)}: Bulk TraverSystem.
     *   All remaining values are traversed in a single bulk.
     *
     *   <li>{@code #whileNext(Control)}: Continuation-controlled Bulk TraverSystem.
     *   All remaining values are traversed in a single bulk, with optional early exit.
     * </ul>
     *
     * @param <F> type of 2nd-order traversal action
     */
    sealed interface Traverser<F> extends TraverserSystem.Step<F>, TraverSystem.For<F>, TraverSystem.While<F> {
        
        /**
         * Combined forward traversal operators to pass through an source of values in forward direction.
         *
         * <p>The following traversal operators are available:
         * <ul>
         *   <li>{@code #next(Fn1.Action)}: Single-step TraverSystem.
         *   Each remaining value is traversed one-by-one, via repeated invocations.
         *
         *   <li>{@code #forNext(Fn1.Action)}: Bulk TraverSystem.
         *   All remaining values are traversed in a single bulk.
         *
         *   <li>{@code #whileNext(Control)}: Continuation-controlled Bulk TraverSystem.
         *   All remaining values are traversed in a single bulk, with optional early exit.
         * </ul>
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Next<F> extends TraverSystem.Traverser<F>, TraverSystem.Step.Next<F>, TraverSystem.For.Next<F>, TraverSystem.While.Next<F> {
  
            /**
             * Performs the given action on a current value and returns true to signal
             * active traversal and request another invocation. Otherwise, false is
             * returned without the action being executed. This signals exhaustion
             * in the forward direction of the traversal.
             *
             * @param action to be performed on a present value
             * @return true if the action has been performed
             */
            @Override
            boolean next(F action);
            
            @Override
            void forNext(F action);

            @Override
            <C extends Eval.Control> Fn1.Predicate<C> whileNext(Fn1<C, F> until);
        }
  
        /**
         * Combined backward traversal operators to pass through an source of values in backward direction.
         *
         * <p>The following traversal operators are available:
         * <ul>
         *   <li>{@code #prev(Fn1.Action)}: Single-step TraverSystem.
         *   Each remaining value is traversed one-by-one, via repeated invocations.
         *
         *   <li>{@code #forPrev(Fn1.Action)}: Bulk TraverSystem.
         *   All remaining values are traversed in a single bulk.
         *
         *   <li>{@code #whilePrev(Control)}: Continuation-controlled Bulk TraverSystem.
         *   All remaining values are traversed in a single bulk, with optional early exit.
         * </ul>
         *
         * @param <F> type of 2nd-order traversal action
         */
        non-sealed interface Prev<F> extends TraverSystem.Traverser<F>, TraverSystem.Step.Prev<F>, TraverSystem.For.Prev<F>, TraverSystem.While.Prev<F> {
          
            /**
             * Performs the given action on a current value and returns true to signal
             * active traversal and request another invocation. Otherwise, false is
             * returned without the action being executed. This signals exhaustion
             * in the backward direction of the traversal.
             *
             * @param action to be performed on a present value
             * @return true if the action has been performed
             */
            @Override
            boolean prev(Fn1.Action<? super A> action);
          
            @Override 
            void forPrev(F action);

            @Override 
            <C extends Eval.Control> Fn1.Predicate<C> whilePrev(Fn1<C, F> until);
        }
    }
}
```

The **Traversal System Abstractions** resonate deeply with the **Principles of Program Construction** through their
focus on **interface type abstraction**, composition, and arrangement, aligning with the orthogonal principles of *
*Abstraction of Type Structure**, **Composition of Type Structure**, and **Arrangement of Type Structure**. Here's how
each aspect connects:

### **I. Abstraction of Type Structure**

The **Traversal System Abstractions** exemplify **interface type abstraction** by encapsulating the core behaviors of
traversal (e.g., `next`, `prev`, `forNext`, `whileNext`) behind **uniform interfaces**, separating the **what** from the
**how**. This approach hides the underlying implementation details while providing a clear **protocol** for interaction,
allowing users to traverse a sequence of values without worrying about the specific data structures or traversal
mechanisms.

- **Interface Type Abstraction**: The `Traversal` interfaces define **contracts** for traversal operators (
  e.g., `Step.Next`, `For.Next`, `While.Next`) without specifying how these operations are implemented. This promotes *
  *polymorphic behavior**, where multiple concrete implementations can follow the same contract, allowing different
  traversal strategies or structures to coexist under a common interface.

- **Parametric Abstraction**: The use of **generics** (`<F>`) allows traversal to be **type-parametric**, enabling it to
  work over multiple types while ensuring **type safety**. The **parametric abstraction** ensures that these operations
  are generic and flexible, without being tied to specific data types, allowing for **type-safe reusability**.

- **Behavioral Abstraction**: By abstracting the behavior of **single-step**, **bulk**, and **continuation-controlled**
  traversals, the `Traversal` interfaces define **interaction protocols**. These behaviors can be reused and applied in
  various contexts, independent of any specific traversal implementation.

- **Hierarchy of Concepts**: The **separation of traversal behaviors** into `Step`, `For`, `While`, and `Traverser`
  interfaces creates a **hierarchy** of abstractions that allow developers to focus on essential behaviors (e.g.,
  forward or backward traversal) without worrying about implementation specifics.

---

### **II. Composition of Type Structure**

The **Traversal System Abstractions** utilize **modular composition** through a hierarchy of **mixin interfaces**. Each
interface (`Step.Next`, `For.Next`, `While.Next`) builds on the previous one, creating **incrementally composed**
traversal behaviors.

- **Interface Composition**: The `Traversal` system allows interfaces to be composed incrementally, where **mixins**
  like `Step`, `For`, and `While` provide different aspects of traversal. This modular approach allows a **clear
  separation of concerns**, where each interface handles a specific type of traversal (e.g., single-step, bulk,
  continuation-controlled), and they are combined to form a comprehensive traversal mechanism.

- **Separation of Concerns**: Each interface in the **Traversal System** handles a distinct aspect of traversal. For
  example, `Step.Next` focuses on **single-step traversal**, while `For.Next` manages **bulk traversal**. This *
  *separation of concerns** allows for flexibility in the composition of traversal mechanisms, where developers can
  compose only the needed functionalities.

- **Hierarchical and Scalable**: The **nested interfaces** (`Step.Next`, `For.Next`, `While.Next`) demonstrate a *
  *hierarchical composition**, where traversal behaviors are layered incrementally. This approach supports scalability
  by allowing developers to compose more complex traversal behaviors from simpler, well-defined operations.

---

### **III. Arrangement of Type Structure**

The **Traversal System Abstractions** emphasize a **logical organization** of types through **nesting**, ensuring that
the system remains **modular**, **navigable**, and **scalable**.

- **Hierarchical Composition**: The **nested interface structure** of the `Traversal` system reflects a natural
  hierarchy of traversal behaviors, where each layer builds on the previous one. For example, `Traversal.Traverser.Next`
  inherits from `Traversal.Step.Next`, `Traversal.For.Next`, and `Traversal.While.Next`, encapsulating multiple
  traversal operators within a **logical containment**.

- **Encapsulation**: The **nested interface arrangement** enforces **scope and visibility**, encapsulating specific
  traversal operators within appropriate contexts (e.g., `Step`, `For`, `While`). This ensures that the traversal
  behavior remains modular and encapsulated within the proper scope, promoting clear **containment relationships**.

- **Containment and Namespace Management**: By **nesting interfaces** (
  e.g., `Traversal.Step.Next`, `Traversal.For.Next`), the system enforces clear **containment** of traversal operators
  within the correct structure. This ensures that related operations are contained within a cohesive module, reducing
  ambiguity and enhancing readability.

- **Semantic Clarity in Naming**: The **interface names** within the `Traversal` system (
  e.g., `Next`, `Prev`, `For`, `While`) are semantically meaningful and reflect their roles within the traversal
  hierarchy. This clarity ensures that the system remains easy to navigate and understand, with names corresponding
  naturally to their purpose.

---

### **Orthogonal Complementary Principles**

The **Traversal System Abstractions** align with the **orthogonal principles** of abstraction, composition, and
arrangement:

- **Abstraction**: The `Traversal` system focuses on **abstracting traversal behaviors** behind uniform interfaces,
  allowing for flexible and polymorphic traversal operators, without tying the system to specific implementations.

- **Composition**: The **modular composition** of interfaces (e.g., `Step.Next`, `For.Next`, `While.Next`) supports *
  *scalability and reuse**, where traversal behaviors are built incrementally and composed to form more complex
  operations.

- **Arrangement**: The **hierarchical organization** of the `Traversal` system ensures that types are logically nested,
  reflecting their **containment relationships** and promoting **modularity** and **semantic clarity**.

---

### **Conclusion**

The **Traversal System Abstractions** resonate with the **Principles of Program Construction** by embodying the core
tenets of **abstraction**, **composition**, and **arrangement**. These abstractions promote **flexibility, reusability,
and clarity** in how traversal behaviors are defined, composed, and organized, creating a system that is **modular**, *
*scalable**, and **semantically coherent**. The focus on **interface type abstraction** allows the system to hide
complexity while exposing necessary traversal operators through a clear and navigable type hierarchy.

