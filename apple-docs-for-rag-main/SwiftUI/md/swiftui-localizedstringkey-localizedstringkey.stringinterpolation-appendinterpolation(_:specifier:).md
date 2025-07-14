

- SwiftUI
- LocalizedStringKey
- LocalizedStringKey.StringInterpolation
-  appendInterpolation(\_:specifier:) 

Instance Method

# appendInterpolation(\_:specifier:)

Appends a type, convertible to a string with a format specifier, to a string interpolation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func appendInterpolation(
    _ value: T,
    specifier: String
) where T : _FormatSpecifiable
```

## Parameters 

`value`  

The value to append.

`specifier`  

A format specifier to convert `subject` to a string representation, like `%f` for a Double, or `%x` to create a hexidecimal representation of a UInt32. For a list of available specifier strings, see String Format Specifers.

## Discussion

Don’t call this method directly; it’s used by the compiler when interpreting string interpolations.

## See Also

### Appending to an interpolation

func appendInterpolation(_:)

Appends an attributed string to a string interpolation.

func appendInterpolation(_:format:)

Appends the formatted representation of a nonstring type supported by a corresponding format style.

func appendInterpolation(_:formatter:)

Appends an optionally-formatted instance of an Objective-C subclass to a string interpolation.

func appendInterpolation(Date, style: Text.DateStyle)

Appends a formatted date to a string interpolation.

func appendInterpolation(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Appends a timer interval to a string interpolation.

func appendLiteral(String)

Appends a literal string.

