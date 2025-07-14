

- SwiftUI
- View
-  chartXAxisLabel(\_:position:alignment:spacing:) 

Instance Method

# chartXAxisLabel(\_:position:alignment:spacing:)

Adds x axis label for charts in the view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartXAxisLabel(
    _ labelKey: LocalizedStringKey,
    position: AnnotationPosition = .automatic,
    alignment: Alignment? = nil,
    spacing: CGFloat? = nil
) -> some View
```

Show all declarations

## Parameters 

`labelKey`  

The key for the localized label string.

`position`  

The position of the label.

`alignment`  

The alignment of the label.

`spacing`  

The spacing of the label from the axis markers.

## See Also

### Axis Labels

func chartXAxisLabel&lt;C>(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?, content: () -> C) -> some View

Adds x axis label for charts in the view.

func chartYAxisLabel(_:position:alignment:spacing:)

Adds y axis label for charts in the view.

func chartYAxisLabel&lt;C>(position: AnnotationPosition, alignment: Alignment?, spacing: CGFloat?, content: () -> C) -> some View

Adds y axis label for charts in the view.

