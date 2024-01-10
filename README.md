# Kotlin-RoadMap `v1.0.0-alpha01`

Kotlin v1.9.22

# 1. Types

### **Numbers**

- Integer types
- Floating-point types
- Literal constants for numbers
- Numbers representation on the JVM
- Explicit number conversions
- Operations on numbers
    - Division of integers
    - Bitwise operations
    - Floating-point numbers comparison

### **Unsigned integer types**

- Unsigned arrays and ranges
- Unsigned integers literals
- Use cases
    - Non-goals

### **Booleans**

### **Characters**

### **Strings**

- String literals
    - Escaped strings
    - Multiline strings
- String templates
- String formatting

### **Arrays**

- When to use arrays
- Create arrays
    - Nested arrays
- Access and modify elements
- Work with arrays
    - Pass variable number of arguments to a function
    - Compare arrays
    - Transform arrays
    - Sum
    - Shuffle
    - Convert arrays to collections
- Primitive-type arrays

### **Type checks and casts**

- is and !is operators
- Smart casts
- "Unsafe" cast operator
- "Safe" (nullable) cast operator

=======================================================================================================

# 2. Control Flow

### **Conditions and loops**

- If expression
- When expression
- For loops
- While loops
- Break and continue in loops

### Returns and jumps

- Returns and jumps
- Break and continue labels
- Return to labels

### Exceptions

- Exceptions
- Exception classes
    - Try is an expression
- Checked exceptions
- The Nothing type
- Java interoperability

### Packages and imports

- Packages and imports
- Default imports
- Imports
- Visibility of top-level declarations

=======================================================================================================

# 3. Functions

# **Functions**

- Functions
- Function usage
    - Parameters
    - Default arguments
    - Named arguments
    - Unit-returning functions
    - Single-expression functions
    - Explicit return types
    - Variable number of arguments (varargs)
        - Infix notation
- Function scope
    - Local functions
    - Member functions
- Generic functions
- Tail recursive functions

# **Lambdas**

- Higher-order functions and lambdas
- Higher-order functions
- Function types
    - Instantiating a function type
    - Invoking a function type instance
    - Inline functions
- Lambda expressions and anonymous functions
    - Lambda expression syntax
    - Passing trailing lambdas
    - it: implicit name of a single parameter
    - Returning a value from a lambda expression
    - Underscore for unused variables
    - Destructuring in lambdas
    - Anonymous functions
    - Closures
    - Function literals with receiver
 
# **Inline functions**

- Inline functions
- noinline
- Non-local returns
- Reified type parameters
- Inline properties
- Restrictions for public API inline functions

# **Operator overloading**

- Operator overloading
- Unary operations
    - Unary prefix operators
    - Increments and decrements
- Binary operations
    - Arithmetic operators
    - in operator
    - Indexed access operator
    - invoke operator
    - Augmented assignments
    - Equality and inequality operators
    - Comparison operators
    - Property delegation operators
- Infix calls for named functions

# **Builders**

- Type-safe builders
- How it works
- Scope control: @DslMarker
- Full definition of the com.example.html package

- Using builders with builder type inference
- Writing your own builders
    - Requirements for enabling builder inference
    - Supported features
- How builder inference works
    - Postponed type variables
    - Contributing to builder inference results

=======================================================================================================

# 4. Classes

- Constructors
    - Secondary constructors
- Creating instances of classes
- Class members
- Inheritance
- Abstract classes
- Companion object

# **Inheritance**

- Overriding methods
- Overriding properties
- Derived class initialization order
- Calling the superclass implementation
- Overriding rules

# **Properties**

- Properties
- Declaring properties
- Getters and setters
    - Backing fields
    - Backing properties
- Compile-time constants
- Late-initialized properties and variables
    - Checking whether a lateinit var is initialized
- Overriding properties
- Delegated properties

# **Interfaces**

- Interfaces
- Implementing interfaces
- Properties in interfaces
- Interfaces Inheritance
- Resolving overriding conflicts

# **Functional (SAM) interfaces**

- Functional (SAM) interfaces
- SAM conversions
- Migration from an interface with constructor function to a functional interface
- Functional interfaces vs. type aliases

# **Visibility modifiers**

- Visibility modifiers
- Packages
- Class members
    - Constructors
    - Local declarations
- Modules

# **Extensions**

- Extensions
- Extension functions
- Extensions are resolved statically
- Nullable receiver
- Extension properties
- Companion object extensions
- Scope of extensions
- Declaring extensions as members
- Note on visibility

# **Data classes**

- Data classes
- Properties declared in the class body
- Copying
- Data classes and destructuring declarations
- Standard data classes

# **Sealed classes and interfaces**

- Sealed classes and interfaces
- Location of direct subclasses
    - Inheritance in multiplatform projects
- Sealed classes and when expression

# **Generics: in, out, where**

- Generics: in, out, where
- Variance
    - Declaration-site variance
- Type projections
    - Use-site variance: type projections
    - Star-projections
- Generic functions
- Generic constraints
    - Upper bounds
- Definitely non-nullable types
- Type erasure
    - Generics type checks and casts
    - Unchecked casts
- Underscore operator for type arguments

# **Nested and inner classes**

- Nested and inner classes
- Inner classes
- Anonymous inner classes

# **Enum classes**

- Enum classes
- Anonymous classes
- Implementing interfaces in enum classes
- Working with enum constants

# **Inline value classes**

- Inline value classes
- Members
- Inheritance
- Representation
    - Mangling
    - Calling from Java code
- Inline classes vs type aliases
- Inline classes and delegation

# **Object expressions and declarations**

- Object expressions and declarations
- Object expressions
    - Creating anonymous objects from scratch
    - Inheriting anonymous objects from supertypes
    - Using anonymous objects as return and value types
    - Accessing variables from anonymous objects
- Object declarations
    - Data objects
    - Companion objects
    - Semantic difference between object expressions and declarations
 
# **Delegation**

- Delegation
- Overriding a member of an interface implemented by delegation

# **Delegated properties**

- Delegated properties
- Standard delegates
    - Lazy properties
    - Observable properties
- Delegating to another property
- Storing properties in a map
- Local delegated properties
- Property delegate requirements
- Translation rules for delegated properties
    - Optimized cases for delegated properties
    - Translation rules when delegating to another property
- Providing a delegate

# **Type aliases**

=======================================================================================================

# 5. Null safety

- Null safety
- Nullable types and non-nullable types
- Checking for null in conditions
- Safe calls
- Nullable receiver
- Elvis operator
- The !! operator
- Safe casts
- Collections of a nullable type

=======================================================================================================

# 6. Equality

- Equality
- Structural equality
- Referential equality
- Floating-point numbers equality
- Array equality

=======================================================================================================

# 7. This expressions

- This expressions
- Qualified this
- Implicit this

=======================================================================================================

# 8. Scope functions

- Scope functions
- Function selection
- Distinctions
    - Context object: this or it
    - Return value
- Functions
    - let
    - with
    - run
    - apply
    - also
- takeIf and takeUnless

=======================================================================================================

# 9. Destructuring declarations

- Destructuring declarations
- Example: returning two values from a function
- Example: destructuring declarations and maps
- Underscore for unused variables
- Destructuring in lambdas

=======================================================================================================

# 10. Reflection

- Reflection
- JVM dependency
- Class references
    - Bound class references
- Callable references
    - Function references
    - Property references
    - Interoperability with Java reflection
    - Constructor references
    - Bound function and property references
    - Bound constructor references
 
=======================================================================================================

# 11. Time measurement

- Time measurement
- Calculate duration
    - Create duration
    - Get string representation
    - Convert duration
    - Compare duration
    - Break duration into components
- Measure time
    - Measure code execution time
    - Mark moments in time
    - Measure differences in time
- Time sources
    - Default time sources per platform
    - Create time source
 
=======================================================================================================

# 12. Collections

- Collections overview
- Collection types
    - Collection
    - List
    - Set
    - Map
    - ArrayDeque
 
=======================================================================================================

# 13. Opt-in requirements

- Opt-in requirements
- Opt in to using API
    - Propagating opt-in
    - Non-propagating opt-in
- Require opt-in for API
    - Create opt-in requirement annotations
    - Mark API elements
- Opt-in requirements for pre-stable APIs

=======================================================================================================

# 14. Annotations

- Annotations
- Usage
- Constructors
- Instantiation
- Lambdas
- Annotation use-site targets
- Java annotations
    - Arrays as annotation parameters
    - Accessing properties of an annotation instance
    - Ability to not generate JVM 1.8+ annotation targets
- Repeatable annotations

=======================================================================================================


# 15. Asynchronous programming techniques

- Asynchronous programming techniques
- Threading
- Callbacks
- Futures, promises, and others
- Reactive extensions
- CoRoutines

=======================================================================================================

# 16. Collections bi' tık Advance a.k.a E.H.

# **Constructing collections**

- Construct from elements
- Create with collection builder functions
- Empty collections
- Initializer functions for lists
- Concrete type constructors
- Copy
- Invoke functions on other collections

# **Iterators**

- Iterators
- List iterators
- Mutable iterators

# **Ranges and progressions**

- Ranges and progressions
- Progression

# **Sequences**

- Sequences
- Construct
    - From elements
    - From an Iterable
    - From a function
    - From chunks
- Sequence operations
- Sequence processing example
    - Iterable
    - Sequence
 
# **Collection operations overview**

- Extension and member functions
- Common operations
- Write operations

# **Collection transformation operations**

- Map
- Zip
- Associate
- Flatten
- String representation

# **Filtering collections**

- Filter by predicate
- Partition
- Test predicates

# **Plus and minus operators**

# **Grouping**

# **Retrieve collection parts**

- Slice
- Take and drop
- Chunked
- Windowed

# **Retrieve single elements**

- Retrieve by position
- Retrieve by condition
- Retrieve with selector
- Random element
- Check element existence

# **Ordering**

- Ordering
- Natural order
- Custom orders
- Reverse order
- Random order

# **Aggregate operations**

- Aggregate operations
- Fold and reduce

# **Collection write operations**

- Adding elements
- Removing elements
- Updating elements

# **List-specific operations**

- **Retrieve elements by index**
- **Retrieve list parts**
- **Find element positions**
    - **Linear search**
    - **Binary search in sorted lists**
- **List write operations**
    - **Add**
    - **Update**
    - **Remove**
    - **Sort**
 
# **List-specific operations**

- **Retrieve elements by index**
- **Retrieve list parts**
- **Find element positions**
    - **Linear search**
    - **Binary search in sorted lists**
- **List write operations**
    - **Add**
    - **Update**
    - **Remove**
    - **Sort**
 
# **Set-specific operations**

# **Map-specific operations**

- Retrieve keys and values
- Retrieve keys and values
- Filter
- Plus and minus operators
- Map write operations
    - Add and update entries
    - Remove entries

=======================================================================================================

# 17. CoRoutines bi' tık Advance a.k.a E.H.

# **Basics**

- Your first coroutine
    - Structured concurrency
- Extract function refactoring
- Scope builder
- Scope builder and concurrency
- An explicit job
- Coroutines are light-weight

# **Shared mutable state and concurrency**

- The problem
- Volatiles are of no help
- Thread-safe data structures
- Thread confinement fine-grained
- Thread confinement coarse-grained
- Mutual exclusion

# **Cancellation and timeouts**

- Cancelling coroutine execution
- Cancellation is cooperative
- Making computation code cancellable
- Closing resources with finally
- Run non-cancellable block
- Timeout
- Asynchronous timeout and resources

# **Composing suspending functions**

- Sequential by default
- Concurrent using async
- Lazily started async
- Async-style functions
- Structured concurrency with async

# **Coroutine context and dispatchers**

- Dispatchers and threads
- Unconfined vs confined dispatcher
- Debugging coroutines and threads
    - Debugging with IDEA
    - Debugging using logging
- Jumping between threads
- Job in the context
- Children of a coroutine
- Parental responsibilities
- Naming coroutines for debugging
- Combining context elements
- Coroutine scope
    - Thread-local data

# **Asynchronous Flow**

- Representing multiple values
    - Sequences
    - Suspending functions
    - Flows
- Flows are cold
- Flow cancellation basics
- Flow builders
- Intermediate flow operators
    - Transform operator
    - Size-limiting operators
- Terminal flow operators
- Flows are sequential
- Flow context
    - A common pitfall when using withContext
    - flowOn operator
- Buffering
    - Conflation
    - Processing the latest value
- Composing multiple flows
    - Zip
    - Combine
- Flattening flows
    - flatMapConcat
    - flatMapMerge
    - flatMapLatest
- Flow exceptions
    - Collector try and catch
    - Everything is caught
- Exception transparency
    - Transparent catch
    - Catching declaratively
- Flow completion
    - Imperative finally block
    - Declarative handling
    - Successful completion
- Imperative versus declarative
- Launching flow
    - Flow cancellation checks
- Flow and Reactive Streams

# **Channels**

- Channel basics
- Closing and iteration over channels
- Building channel producers
- Pipelines
- Prime numbers with pipeline
- Fan-out
- Fan-in
- Buffered channels
- Channels are fair
- Ticker channels

# **Coroutine exceptions handling**

- Exception propagation
- CoroutineExceptionHandler
- Cancellation and exceptions
- Exceptions aggregation
- Supervision
    - Supervision job
    - Supervision scope

 
License
=======

    Copyright 2013 KeKod v2.0 : BuggyHouse.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
