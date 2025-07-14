

- Swift
- Unicode
- Unicode.ParseResult
-  Unicode.ParseResult.error(length:) 

Case

# Unicode.ParseResult.error(length:)

An encoding error was detected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case error(length: Int)
```

## Discussion

`length` is the number of underlying code units consumed by this error, guaranteed to be greater than 0.

