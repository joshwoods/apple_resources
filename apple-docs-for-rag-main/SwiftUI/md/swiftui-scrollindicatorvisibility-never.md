

- SwiftUI
- ScrollIndicatorVisibility
-  never 

Type Property

# never

Scroll indicators should never be visible.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var never: ScrollIndicatorVisibility { get }
```

## Discussion

This value behaves like hidden, but overrides scrollable views that choose to keep their indidicators visible. When using this value, provide an alternative method of scrolling. The typical horizontal swipe gesture might not be available, depending on the current input device.

## See Also

### Getting visibilties

static var automatic: ScrollIndicatorVisibility

Scroll indicator visibility depends on the policies of the component accepting the visibility configuration.

static var hidden: ScrollIndicatorVisibility

Hide the scroll indicators.

static var visible: ScrollIndicatorVisibility

Show the scroll indicators.

