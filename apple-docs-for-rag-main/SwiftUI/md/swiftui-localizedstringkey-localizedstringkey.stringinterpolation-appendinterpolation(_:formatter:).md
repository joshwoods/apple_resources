

- SwiftUI
- LocalizedStringKey
- LocalizedStringKey.StringInterpolation
-  appendInterpolation(\_:formatter:) 

Instance Method

# appendInterpolation(\_:formatter:)

Appends an optionally-formatted instance of an Objective-C subclass to a string interpolation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func appendInterpolation(
    _ subject: Subject,
    formatter: Formatter? = nil
) where Subject : NSObject
```

Show all declarations

## Parameters 

`subject`  

An NSObject to append.

`formatter`  

A formatter to convert `subject` to a string representation.

## Discussion

Don’t call this method directly; it’s used by the compiler when interpreting string interpolations.

The following example shows how to use a Measurement value and a MeasurementFormatter to create a LocalizedStringKey that uses the formatter style Formatter.UnitStyle.long when generating the measurement’s string representation. Rather than calling `appendInterpolation(_:formatter)` directly, the code gets the formatting behavior implicitly by using the `\()` string interpolation syntax.

```
let siResistance = Measurement(value: 640, unit: UnitElectricResistance.ohms)
let formatter = MeasurementFormatter()
formatter.unitStyle = .long
let key = LocalizedStringKey ("Resistance: \(siResistance, formatter: formatter)")
let text1 = Text(key) // Text contains "Resistance: 640 ohms"
```

## See Also

### Appending to an interpolation

func appendInterpolation(_:)

Appends an attributed string to a string interpolation.

func appendInterpolation&lt;T>(T, specifier: String)

Appends a type, convertible to a string with a format specifier, to a string interpolation.

func appendInterpolation(_:format:)

Appends the formatted representation of a nonstring type supported by a corresponding format style.

func appendInterpolation(Date, style: Text.DateStyle)

Appends a formatted date to a string interpolation.

func appendInterpolation(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Appends a timer interval to a string interpolation.

func appendLiteral(String)

Appends a literal string.

