

- Swift
- Imported C and Objective-C APIs
-  Using Imported C Functions in Swift 

Article

# Using Imported C Functions in Swift

Learn how to call imported functions that are declared in a C header.

## Overview

Swift imports any function declared in a C header as a Swift global function.

For example, consider the following C function declarations:

```
int product(int multiplier, int multiplicand);
int quotient(int dividend, int divisor, int *remainder);

struct Point2D createPoint2D(float x, float y);
float distance(struct Point2D from, struct Point2D to);
```

Here’s how Swift imports them:

```
func product(_ multiplier: Int32, _ multiplicand: Int32) -> Int32
func quotient(_ dividend: Int32, _ divisor: Int32, _ remainder: UnsafeMutablePointer) -> Int32

func createPoint2D(_ x: Float, _ y: Float) -> Point2D
func distance(_ from: Point2D, _ to: Point2D) -> Float
```

### Use a CVaListPointer to Call Variadic Functions

In Swift, you can call C variadic functions, such as `vasprintf(_:_:_:)`, using the Swift getVaList(_:) or withVaList(_:_:) functions. The `withVaList(_:_:)` function takes an array of CVarArg values and provides a CVaListPointer value within the body of a closure parameter, whereas the `getVaList(_:)` function returns this value directly. With either function, you pass the resulting `CVaListPointer` value as the `va_list` argument of the C variadic function.

For example, here’s how to call the `vasprintf(_:_:_:)` function in Swift:

```
func swiftprintf(format: String, arguments: CVarArg...) -> String? {
    return withVaList(arguments) { va_list in
        var buffer: UnsafeMutablePointer? = nil
        return format.withCString { cString in
            guard vasprintf(&buffer, cString, va_list) != 0 else {
                return nil
            }

            return String(validatingUTF8: buffer!)
        }
    }
}
print(swiftprintf(format: "√2 ≅ %g", arguments: sqrt(2.0))!)
// Prints "√2 ≅ 1.41421"
```

Swift only imports C variadic functions that use a `va_list` for their arguments. C functions that use the `...` syntax for variadic arguments are not imported, and therefore can’t be called using `CVarArg` arguments.

### Call Functions with Pointer Parameters

Whenever possible, Swift avoids giving you direct access to pointers. When importing C function parameters, however, Swift maps pointer parameters to standard library pointer types. The following tables use `Type` as a placeholder type name to indicate syntax for the mappings.

For return types, variables, and arguments, the following mappings apply:

| C Syntax | Swift Syntax |
|----|----|
| `const Type *` | UnsafePointer\ |
| `Type *` | UnsafeMutablePointer\ |

For class types, the following mappings apply:

| C Syntax | Swift Syntax |
|----|----|
| `Type * const *` | UnsafePointer\ |
| `Type * __strong *` | UnsafeMutablePointer\ |
| `Type **` | AutoreleasingUnsafeMutablePointer\ |

For pointers to untyped, raw memory, the following mappings apply:

| C Syntax | Swift Syntax |
|----|----|
| `const void *` | UnsafeRawPointer |
| `void *` | UnsafeMutableRawPointer |

C function pointers are imported into Swift as closures with the C function pointer calling convention, denoted by the `@convention(c)` attribute. For example, a function pointer that has the type `int (*)(void)` in C is imported into Swift as `@convention(c) () -> Int32`.

If the type of the value pointed to by a C pointer cannot be represented by Swift, as is the case with an incomplete struct type, the pointer is imported as an `OpaquePointer`.

## See Also

### C APIs

Using Imported C Structs and Unions in Swift

Learn how Swift represents imported C structures and unions, including types with bitfields and unnamed fields.

Using Imported C Macros in Swift

Use imported C-defined macros as constants.

