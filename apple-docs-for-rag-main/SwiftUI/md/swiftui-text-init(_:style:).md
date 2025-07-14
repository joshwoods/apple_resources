

- SwiftUI
- Text
-  init(\_:style:) 

Initializer

# init(\_:style:)

Creates an instance that displays localized dates and times using a specific style.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    _ date: Date,
    style: Text.DateStyle
)
```

## Parameters 

`date`  

The target date to display.

`style`  

The style used when displaying a date.

## See Also

### Creating a text view

init(LocalizedStringKey, tableName: String?, bundle: Bundle?, comment: StaticString?)

Creates a text view that displays localized content identified by a key.

init(_:)

Creates a text view that displays styled attributed content.

init(verbatim: String)

Creates a text view that displays a string literal without localization.

init(_:format:)

Creates a text view that displays the formatted representation of a nonstring type supported by a corresponding format style.

init(_:formatter:)

Creates a text view that displays the formatted representation of a Foundation object.

init(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Creates an instance that displays a timer counting within the provided interval.

