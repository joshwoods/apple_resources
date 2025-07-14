

- Swift
- BinaryInteger
-  formatted(\_:) 

Instance Method

# formatted(\_:)

Format `self` with the given format. `self` is first converted to `S.FormatInput` type, then format with the given format.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted(_ format: S) -> S.FormatOutput where S : FormatStyle, S.FormatInput : BinaryInteger
```

