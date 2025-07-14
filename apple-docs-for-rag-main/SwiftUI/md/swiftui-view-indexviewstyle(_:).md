

- SwiftUI
- View
-  indexViewStyle(\_:) 

Instance Method

# indexViewStyle(\_:)

Sets the style for the index view within the current environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func indexViewStyle(_ style: S) -> some View where S : IndexViewStyle
```

## Parameters 

`style`  

The style to apply to this view.

## See Also

### Styling groups

func controlGroupStyle&lt;S>(S) -> some View

Sets the style for control groups within this view.

protocol ControlGroupStyle

Defines the implementation of all control groups within a view hierarchy.

struct ControlGroupStyleConfiguration

The properties of a control group.

func formStyle&lt;S>(S) -> some View

Sets the style for forms in a view hierarchy.

protocol FormStyle

The appearance and behavior of a form.

struct FormStyleConfiguration

The properties of a form instance.

func groupBoxStyle&lt;S>(S) -> some View

Sets the style for group boxes within this view.

protocol GroupBoxStyle

A type that specifies the appearance and interaction of all group boxes within a view hierarchy.

struct GroupBoxStyleConfiguration

The properties of a group box instance.

protocol IndexViewStyle

Defines the implementation of all `IndexView` instances within a view hierarchy.

func labeledContentStyle&lt;S>(S) -> some View

Sets a style for labeled content.

protocol LabeledContentStyle

The appearance and behavior of a labeled content instance..

struct LabeledContentStyleConfiguration

The properties of a labeled content instance.

