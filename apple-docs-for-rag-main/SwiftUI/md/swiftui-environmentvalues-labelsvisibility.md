

- SwiftUI
- EnvironmentValues
-  labelsVisibility 

Instance Property

# labelsVisibility

The labels visibility set by labelsVisibility(_:).

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var labelsVisibility: Visibility { get set }
```

## Discussion

Read this environment value from within a view to obtain the preferred visibility for labels within the hierarchy. If you would like to dynamically hide the label of your custom view, make sure to include an accessibility label via the accessibilityLabel(content:) modifier as illustrated below:

```
@Environment(\.labelsVisibility)
private var labelsVisibility

var body: some View {
    VStack {
        QuizCardView()
        if labelsVisibility != .hidden {
            label
        }
    }
    .accessibilityLabel {
        label
    }
}

private var label: some View {
    Text("Quiz Card")
}
```

## See Also

### Hiding system elements

func labelsHidden() -> some View

Hides the labels of any controls contained within this view.

func labelsVisibility(Visibility) -> some View

Controls the visibility of labels of any controls contained within this view.

func menuIndicator(Visibility) -> some View

Sets the menu indicator visibility for controls within this view.

func statusBarHidden(Bool) -> some View

Sets the visibility of the status bar.

func persistentSystemOverlays(Visibility) -> some View

Sets the preferred visibility of the non-transient system views overlaying the app.

enum Visibility

The visibility of a UI element, chosen automatically based on the platform, current context, and other factors.

