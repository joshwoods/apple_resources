

- Swift
-  ExpressibleByArrayLiteral 

Protocol

# ExpressibleByArrayLiteral

A type that can be initialized using an array literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByArrayLiteral
```

## Overview

An array literal is a simple way of expressing a list of values. Simply surround a comma-separated list of values, instances, or literals with square brackets to create an array literal. You can use an array literal anywhere an instance of an `ExpressibleByArrayLiteral` type is expected: as a value assigned to a variable or constant, as a parameter to a method or initializer, or even as the subject of a nonmutating operation like `map(_:)` or `filter(_:)`.

Arrays, sets, and option sets all conform to `ExpressibleByArrayLiteral`, and your own custom types can as well. Here’s an example of creating a set and an array using array literals:

```
let employeesSet: Set = ["Amir", "Jihye", "Dave", "Alessia", "Dave"]
print(employeesSet)
// Prints "["Amir", "Dave", "Jihye", "Alessia"]"

let employeesArray: [String] = ["Amir", "Jihye", "Dave", "Alessia", "Dave"]
print(employeesArray)
// Prints "["Amir", "Jihye", "Dave", "Alessia", "Dave"]"
```

The `Set` and `Array` types each handle array literals in their own way to create new instances. In this case, the newly created set drops the duplicate value (“Dave”) and doesn’t maintain the order of the array literal’s elements. The new array, on the other hand, matches the order and number of elements provided.

Note

An array literal is not the same as an `Array` instance. You can’t initialize a type that conforms to `ExpressibleByArrayLiteral` simply by assigning an existing array.

```
let anotherSet: Set = employeesArray
// error: cannot convert value of type '[String]' to specified type 'Set'
```

# Type Inference of Array Literals

Whenever possible, Swift’s compiler infers the full intended type of your array literal. Because `Array` is the default type for an array literal, without writing any other code, you can declare an array with a particular element type by providing one or more values.

In this example, the compiler infers the full type of each array literal.

```
let integers = [1, 2, 3]
// 'integers' has type '[Int]'

let strings = ["a", "b", "c"]
// 'strings' has type '[String]'
```

An empty array literal alone doesn’t provide enough information for the compiler to infer the intended type of the `Array` instance. When using an empty array literal, specify the type of the variable or constant.

```
var emptyArray: [Bool] = []
// 'emptyArray' has type '[Bool]'
```

Because many functions and initializers fully specify the types of their parameters, you can often use an array literal with or without elements as a parameter. For example, the `sum(_:)` function shown here takes an `Int` array as a parameter:

```
func sum(values: [Int]) -> Int {
    return values.reduce(0, +)
}

let sumOfFour = sum([5, 10, 15, 20])
// 'sumOfFour' == 50

let sumOfNone = sum([])
// 'sumOfNone' == 0
```

When you call a function that does not fully specify its parameters’ types, use the type-cast operator (`as`) to specify the type of an array literal. For example, the `log(name:value:)` function shown here has an unconstrained generic `value` parameter.

```
func log(name name: String, value: T) {
    print("\(name): \(value)")
}

log(name: "Four integers", value: [5, 10, 15, 20])
// Prints "Four integers: [5, 10, 15, 20]"

log(name: "Zero integers", value: [] as [Int])
// Prints "Zero integers: []"
```

# Conforming to ExpressibleByArrayLiteral

Add the capability to be initialized with an array literal to your own custom types by declaring an `init(arrayLiteral:)` initializer. The following example shows the array literal initializer for a hypothetical `OrderedSet` type, which has setlike semantics but maintains the order of its elements.

```
struct OrderedSet: Collection, SetAlgebra {
    // implementation details
}

extension OrderedSet: ExpressibleByArrayLiteral {
    init(arrayLiteral: Element...) {
        self.init()
        for element in arrayLiteral {
            self.append(element)
        }
    }
}
```

## Topics

### Associated Types

associatedtype ArrayLiteralElement

The type of the elements of an array literal.

**Required**

### Initializers

init(arrayLiteral: Self.ArrayLiteralElement...)

Creates an instance initialized with the given elements.

**Required** Default implementations provided.

## Relationships

### Inherited By

- OptionSet
- SIMD
- SetAlgebra

### Conforming Types

- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- SIMD16
- SIMD2
- SIMD3
- SIMD32
- SIMD4
- SIMD64
- SIMD8
- SIMDMask
- Set

  Conforms when `Element` conforms to `Hashable`.

## See Also

### Collection Literals

protocol ExpressibleByDictionaryLiteral

A type that can be initialized using a dictionary literal.

