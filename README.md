# Best practices

#### When you find yourself writing nearly repeated code, try to abstract instead.

#### DRY (don’t repeat yourself)

#### Strategy design pattern which lets you define a family of algorithms, encapsulate each algorithm (called a strategy), and select an algorithm at run time

#### Behavior parameterization: The ability to tell a method to take multiple behaviors (or strategies) as parameters and use them inter-nally to accomplish different behaviors.

#### You need abstract over behavior and make your code adapt to require-ment changes

#### Single Responsibility

#### Open/Closed

#### Liskov Substitution

#### Interface Segregation

#### Dependency Inversion

# Facts

#### Boxed values are a wrapper around primitive types and are stored on the heap.

#### Therefore

#### boxed values use more memory and require additional memory lookups to fetch the wrapped primitive value.

# Common functional interfaces added in Java 8

| Interface           | Signature      |
|---------------------|----------------|
| Predicate<T>        | T -> boolean   |
| Consumer<T>         | T -> void      |
| Function<T, R>      | T->R           |
| Supplier<T>         | () -> T        |
| UnaryOperator<T>    | T->T           |
| BinaryOperator<T>   | (T,T)->T       |
| BiPredicate<T, U>   | (T,U)->boolean |
| BiConsumer<T, U>    | (T,U)->void    |
| BiFunction<T, U, R> | (T,U)->R       |

#### Type inference

| Interface              | Signature                                                                               |
|------------------------|-----------------------------------------------------------------------------------------|
| Without type inference | Comparator<Apple> c = (Apple a1, Apple a2) -> a1.getWeight().compareTo(a2.getWeight()); |
| With type inference    | Comparator<Apple> c = (a1, a2) -> a1.getWeight().compareTo(a2.getWeight());             |