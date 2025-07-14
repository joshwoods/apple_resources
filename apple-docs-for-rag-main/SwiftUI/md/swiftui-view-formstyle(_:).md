

- SwiftUI
- View
-  formStyle(\_:) 

Instance Method

# formStyle(\_:)

Sets the style for forms in a view hierarchy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func formStyle(_ style: S) -> some View where S : FormStyle
```

## Parameters 

`style`  

The form style to set.

## Return Value

A view that uses the specified form style for itself and its child views.

## See Also

### Grouping inputs

struct Form

A container for grouping controls used for data entry, such as in settings or inspectors.

struct LabeledContent

A container for attaching a label to a value-bearing view.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

