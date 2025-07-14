

- SwiftUI
- View
-  statusBarHidden(\_:) 

Instance Method

# statusBarHidden(\_:)

Sets the visibility of the status bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
nonisolated
func statusBarHidden(_ hidden: Bool = true) -> some View
```

## Parameters 

`hidden`  

A Boolean value that indicates whether to hide the status bar.

## See Also

### Hiding system elements

func labelsHidden() -> some View

Hides the labels of any controls contained within this view.

func labelsVisibility(Visibility) -> some View

Controls the visibility of labels of any controls contained within this view.

var labelsVisibility: Visibility

The labels visibility set by labelsVisibility(_:).

func menuIndicator(Visibility) -> some View

Sets the menu indicator visibility for controls within this view.

func persistentSystemOverlays(Visibility) -> some View

Sets the preferred visibility of the non-transient system views overlaying the app.

enum Visibility

The visibility of a UI element, chosen automatically based on the platform, current context, and other factors.

