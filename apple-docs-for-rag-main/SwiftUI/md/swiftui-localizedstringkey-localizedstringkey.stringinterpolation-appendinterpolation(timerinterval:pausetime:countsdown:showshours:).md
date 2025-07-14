

- SwiftUI
- LocalizedStringKey
- LocalizedStringKey.StringInterpolation
-  appendInterpolation(timerInterval:pauseTime:countsDown:showsHours:) 

Instance Method

# appendInterpolation(timerInterval:pauseTime:countsDown:showsHours:)

Appends a timer interval to a string interpolation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func appendInterpolation(
    timerInterval: ClosedRange,
    pauseTime: Date? = nil,
    countsDown: Bool = true,
    showsHours: Bool = true
)
```

## Parameters 

`timerInterval`  

The interval between where to run the timer.

`pauseTime`  

If present, the date at which to pause the timer. The default is `nil` which indicates to never pause.

`countsDown`  

Whether to count up or down. The default is `true`.

`showsHours`  

Whether to include an hours component if there are more than 60 minutes left on the timer. The default is `true`.

## Discussion

Don’t call this method directly; it’s used by the compiler when interpreting string interpolations.

## See Also

### Appending to an interpolation

func appendInterpolation(_:)

Appends an attributed string to a string interpolation.

func appendInterpolation&lt;T>(T, specifier: String)

Appends a type, convertible to a string with a format specifier, to a string interpolation.

func appendInterpolation(_:format:)

Appends the formatted representation of a nonstring type supported by a corresponding format style.

func appendInterpolation(_:formatter:)

Appends an optionally-formatted instance of an Objective-C subclass to a string interpolation.

func appendInterpolation(Date, style: Text.DateStyle)

Appends a formatted date to a string interpolation.

func appendLiteral(String)

Appends a literal string.

