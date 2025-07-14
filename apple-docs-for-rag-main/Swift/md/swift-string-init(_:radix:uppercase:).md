

- Swift
- String
-  init(\_:radix:uppercase:) 

Initializer

# init(\_:radix:uppercase:)

Creates a string representing the given value in base 10, or some other specified base.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    _ value: T,
    radix: Int = 10,
    uppercase: Bool = false
) where T : BinaryInteger
```

## Parameters 

`value`  

The value to convert to a string.

`radix`  

The base to use for the string representation. `radix` must be at least 2 and at most 36. The default is 10.

`uppercase`  

Pass `true` to use uppercase letters to represent numerals greater than 9, or `false` to use lowercase letters. The default is `false`.

## Discussion

The following example converts the maximal `Int` value to a string and prints its length:

```
let max = String(Int.max)
print("\(max) has \(max.count) digits.")
// Prints "9223372036854775807 has 19 digits."
```

Numerals greater than 9 are represented as Roman letters. These letters start with `"A"` if `uppercase` is `true`; otherwise, with `"a"`.

```
let v = 999_999
print(String(v, radix: 2))
// Prints "11110100001000111111"

print(String(v, radix: 16))
// Prints "f423f"
print(String(v, radix: 16, uppercase: true))
// Prints "F423F"
```

