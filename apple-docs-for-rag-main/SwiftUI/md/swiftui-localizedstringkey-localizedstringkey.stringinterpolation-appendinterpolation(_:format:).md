

- SwiftUI
- LocalizedStringKey
- LocalizedStringKey.StringInterpolation
-  appendInterpolation(\_:format:) 

Instance Method

# appendInterpolation(\_:format:)

Appends the formatted representation of a nonstring type supported by a corresponding format style.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func appendInterpolation(
    _ input: F.FormatInput,
    format: F
) where F : FormatStyle, F.FormatInput : Equatable, F.FormatOutput == AttributedString
```

Show all declarations

## Parameters 

`input`  

The instance to format and append.

`format`  

A format style to use when converting `input` into an attributed string representation.

## Discussion

Don’t call this method directly; it’s used by the compiler when interpreting string interpolations.

The following example shows how to use a string interpolation to format a Date with a Date.FormatStyle and append it to static text. The resulting interpolation implicitly creates a LocalizedStringKey, which a Text uses to provide its content.

```
Text("The time is \(myDate, format: Date.FormatStyle(date: .omitted, time:.complete).attributedStyle)")
```

## See Also

### Appending to an interpolation

func appendInterpolation(_:)

Appends an attributed string to a string interpolation.

func appendInterpolation&lt;T>(T, specifier: String)

Appends a type, convertible to a string with a format specifier, to a string interpolation.

func appendInterpolation(_:formatter:)

Appends an optionally-formatted instance of an Objective-C subclass to a string interpolation.

func appendInterpolation(Date, style: Text.DateStyle)

Appends a formatted date to a string interpolation.

func appendInterpolation(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Appends a timer interval to a string interpolation.

func appendLiteral(String)

Appends a literal string.

