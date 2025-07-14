

- SwiftUI
- EnvironmentValues
-  horizontalScrollIndicatorVisibility 

Instance Property

# horizontalScrollIndicatorVisibility

The visibility to apply to scroll indicators of any horizontally scrollable content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var horizontalScrollIndicatorVisibility: ScrollIndicatorVisibility { get set }
```

## See Also

### Showing scroll indicators

func scrollIndicatorsFlash(onAppear: Bool) -> some View

Flashes the scroll indicators of a scrollable view when it appears.

func scrollIndicatorsFlash(trigger: some Equatable) -> some View

Flashes the scroll indicators of scrollable views when a value changes.

func scrollIndicators(ScrollIndicatorVisibility, axes: Axis.Set) -> some View

Sets the visibility of scroll indicators within this view.

var verticalScrollIndicatorVisibility: ScrollIndicatorVisibility

The visiblity to apply to scroll indicators of any vertically scrollable content.

struct ScrollIndicatorVisibility

The visibility of scroll indicators of a UI element.

