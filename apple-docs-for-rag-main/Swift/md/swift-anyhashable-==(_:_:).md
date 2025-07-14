

- Swift
- AnyHashable
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two type-erased hashable instances wrap the same value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func == (lhs: AnyHashable, rhs: AnyHashable) -> Bool
```

## Parameters 

`lhs`  

A type-erased hashable value.

`rhs`  

Another type-erased hashable value.

## Discussion

`AnyHashable` considers bridged counterparts (such as a `String` and an `NSString`) of the same value to be equivalent when type-erased. If those compatible types use different definitions for equality, values that were originally distinct might compare as equal when they are converted to `AnyHashable`:

```
let string1 = "café"
let string2 = "cafe\u{301}" // U+301 COMBINING ACUTE ACCENT
let nsString1 = string1 as NSString
let nsString2 = string2 as NSString
let typeErased1 = nsString1 as AnyHashable
let typeErased2 = nsString2 as AnyHashable
print(string1 == string2)         // prints "true"
print(nsString1 == nsString2)     // prints "false"
print(typeErased1 == typeErased2) // prints "true"
```

