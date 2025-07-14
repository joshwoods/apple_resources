

- SwiftUI
- Text
-  init(\_:format:) 

Initializer

# init(\_:format:)

Creates a text view that displays the formatted representation of a nonstring type supported by a corresponding format style.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ input: F.FormatInput,
    format: F
) where F : FormatStyle, F.FormatInput : Equatable, F.FormatOutput == AttributedString
```

Show all declarations

## Parameters 

`input`  

The underlying value to display.

`format`  

A format style of type `F` to convert the underlying value of type `F.FormatInput` to an attributed string representation.

## Discussion

Use this initializer to create a text view backed by a nonstring value, using a FormatStyle to convert the type to an attributed string representation. Any changes to the value update the string displayed by the text view.

In the following example, three Text views present a date with different combinations of date and time fields, by using different Date.FormatStyle options.

```
@State private var myDate = Date()
var body: some View {
    VStack {
        Text(myDate, format: Date.FormatStyle(date: .numeric, time: .omitted).attributedStyle)
        Text(myDate, format: Date.FormatStyle(date: .complete, time: .complete).attributedStyle)
        Text(myDate, format: Date.FormatStyle().hour(.defaultDigitsNoAMPM).minute().attributedStyle)
    }
}
```

## See Also

### Creating a text view

init(LocalizedStringKey, tableName: String?, bundle: Bundle?, comment: StaticString?)

Creates a text view that displays localized content identified by a key.

init(_:)

Creates a text view that displays styled attributed content.

init(verbatim: String)

Creates a text view that displays a string literal without localization.

init(Date, style: Text.DateStyle)

Creates an instance that displays localized dates and times using a specific style.

init(_:formatter:)

Creates a text view that displays the formatted representation of a Foundation object.

init(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Creates an instance that displays a timer counting within the provided interval.

