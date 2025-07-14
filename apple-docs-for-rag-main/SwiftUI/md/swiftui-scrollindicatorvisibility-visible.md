

- SwiftUI
- ScrollIndicatorVisibility
-  visible 

Type Property

# visible

Show the scroll indicators.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var visible: ScrollIndicatorVisibility { get }
```

## Discussion

The actual visibility of the indicators depends on platform conventions like auto-hiding behaviors in iOS or user preference behaviors in macOS.

## See Also

### Getting visibilties

static var automatic: ScrollIndicatorVisibility

Scroll indicator visibility depends on the policies of the component accepting the visibility configuration.

static var hidden: ScrollIndicatorVisibility

Hide the scroll indicators.

static var never: ScrollIndicatorVisibility

Scroll indicators should never be visible.

