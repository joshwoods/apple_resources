

- SwiftUI
- WidgetConfiguration
-  configurationDisplayName(\_:) 

Instance Method

# configurationDisplayName(\_:)

Sets the name shown for a widget when a user adds or edits it using the contents of a text view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func configurationDisplayName(_ displayName: Text) -> some WidgetConfiguration
```

Show all declarations

## Parameters 

`displayName`  

A text view containing a localized string to display.

## Return Value

A widget configuration with a descriptive name for the widget.

