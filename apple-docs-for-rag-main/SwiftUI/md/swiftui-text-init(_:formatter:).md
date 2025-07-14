

- SwiftUI
- Text
-  init(\_:formatter:) 

Initializer

# init(\_:formatter:)

Creates a text view that displays the formatted representation of a Foundation object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    _ subject: Subject,
    formatter: Formatter
) where Subject : NSObject
```

Show all declarations

## Parameters 

`subject`  

An NSObject instance compatible with `formatter`.

`formatter`  

A Formatter capable of converting `subject` into a string representation.

## Discussion

Use this initializer to create a text view that formats `subject` using `formatter`.

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

init(_:format:)

Creates a text view that displays the formatted representation of a nonstring type supported by a corresponding format style.

init(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Creates an instance that displays a timer counting within the provided interval.

