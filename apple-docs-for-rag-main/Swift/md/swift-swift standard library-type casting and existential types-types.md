

- Swift
- Swift Standard Library
-  Type Casting and Existential Types 

API Collection

# Type Casting and Existential Types

Perform casts between types or represent values of any type.

## Topics

### Integer Value Casting

func numericCast&lt;T, U>(T) -> U

Returns the given integer as the equivalent value in a different integer type.

### Closure Casting

func withoutActuallyEscaping&lt;ClosureType, ResultType, Failure>(ClosureType, do: (ClosureType) throws(Failure) -> ResultType) throws(Failure) -> ResultType

Allows a nonescaping closure to temporarily be used as if it were allowed to escape.

### Instance Casting

func unsafeDowncast&lt;T>(AnyObject, to: T.Type) -> T

Returns the given instance cast unconditionally to the specified type.

func unsafeBitCast&lt;T, U>(T, to: U.Type) -> U

Returns the bits of the given instance, interpreted as having the specified type.

### Existential Types

Use a variable or constant with an existential type to hold an instance of any type.

typealias AnyObject

The protocol to which all classes implicitly conform.

typealias AnyClass

The protocol to which all class types implicitly conform.

### Comparing Identity

func === (AnyObject?, AnyObject?) -> Bool

func !== (AnyObject?, AnyObject?) -> Bool

### Void Type

typealias Void

The return type of functions that don’t explicitly specify a return type, that is, an empty tuple `()`.

## See Also

### Programming Tasks

Input and Output

Print values to the console, read from and write to text streams, and use command line arguments.

Debugging and Reflection

Fortify your code with runtime checks, and examine your values’ runtime representation.

Macros

Generate boilerplate code and perform other compile-time operations.

Concurrency

Perform asynchronous and parallel operations.

Key-Path Expressions

Use key-path expressions to access properties dynamically.

Manual Memory Management

Allocate and manage memory manually.

C Interoperability

Use imported C types or call C variadic functions.

Operator Declarations

Work with prefix, postfix, and infix operators.

