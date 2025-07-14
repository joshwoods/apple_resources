

- SwiftUI
- LocalizedStringKey
- LocalizedStringKey.StringInterpolation
-  appendInterpolation(\_:) 

Instance Method

# appendInterpolation(\_:)

Appends an attributed string to a string interpolation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func appendInterpolation(_ attributedString: AttributedString)
```

Show all declarations

## Parameters 

`attributedString`  

The attributed string to append.

## Discussion

Don’t call this method directly; it’s used by the compiler when interpreting string interpolations.

The following example shows how to use a string interpolation to format an AttributedString and append it to static text. The resulting interpolation implicitly creates a LocalizedStringKey, which a Text view uses to provide its content.

```
struct ContentView: View {

    var nextDate: AttributedString {
        var result = Calendar.current
            .nextWeekend(startingAfter: Date.now)!
            .start
            .formatted(
                .dateTime
                .month(.wide)
                .day()
                .attributed
            )
        result.backgroundColor = .green
        result.foregroundColor = .white
        return result
    }

    var body: some View {
        Text("Our next catch-up is on \(nextDate)!")
    }
}
```

For this example, assume that the app runs on a device set to a Russian locale, and has the following entry in a Russian-localized `Localizable.strings` file:

```
"Our next catch-up is on %@!" = "Наша следующая встреча состоится %@!";
```

The attributed string `nextDate` replaces the format specifier `%@`, maintaining its color and date-formatting attributes, when the Text view renders its contents:

## See Also

### Appending to an interpolation

func appendInterpolation&lt;T>(T, specifier: String)

Appends a type, convertible to a string with a format specifier, to a string interpolation.

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

