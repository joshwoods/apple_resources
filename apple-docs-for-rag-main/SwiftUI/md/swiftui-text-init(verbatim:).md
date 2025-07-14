

- SwiftUI
- Text
-  init(verbatim:) 

Initializer

# init(verbatim:)

Creates a text view that displays a string literal without localization.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(verbatim content: String)
```

## Parameters 

`content`  

A string to display without localization.

## Discussion

Use this initializer to create a text view with a string literal without performing localization:

```
Text(verbatim: "pencil") // Displays the string "pencil" in any locale.
```

If you want to localize a string literal before displaying it, use the init(_:tableName:bundle:comment:) initializer instead. If you want to display a string variable, use the init(_:) initializer, which also bypasses localization.

## See Also

### Creating a text view

init(LocalizedStringKey, tableName: String?, bundle: Bundle?, comment: StaticString?)

Creates a text view that displays localized content identified by a key.

init(_:)

Creates a text view that displays styled attributed content.

init(Date, style: Text.DateStyle)

Creates an instance that displays localized dates and times using a specific style.

init(_:format:)

Creates a text view that displays the formatted representation of a nonstring type supported by a corresponding format style.

init(_:formatter:)

Creates a text view that displays the formatted representation of a Foundation object.

init(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Creates an instance that displays a timer counting within the provided interval.

