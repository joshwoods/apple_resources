

- SwiftUI
- ProgressView
-  init(\_:) 

Initializer

# init(\_:)

Creates a progress view for showing indeterminate progress that generates its label from a localized string.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(_ titleKey: LocalizedStringKey) where Label == Text
```

Available when `Label` conforms to `View` and `CurrentValueLabel` is `EmptyView`.

Show all declarations

## Parameters 

`titleKey`  

The key for the progress view’s localized title that describes the task in progress.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings. To initialize a indeterminate progress view with a string variable, use the corresponding initializer that takes a `StringProtocol` instance.

## See Also

### Creating an indeterminate progress view

init()

Creates a progress view for showing indeterminate progress, without a label.

init(label: () -> Label)

Creates a progress view for showing indeterminate progress that displays a custom label.

init&lt;S>(S)

Creates a progress view for showing indeterminate progress that generates its label from a string.

