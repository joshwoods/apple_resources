

- Swift
- Int128
-  Int128.Words 

Type Alias

# Int128.Words

A type that represents the words of a binary integer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias Words = UInt128.Words
```

## Discussion

The `Words` type must conform to the `RandomAccessCollection` protocol with an `Element` type of `UInt` and `Index` type of `Int`.

