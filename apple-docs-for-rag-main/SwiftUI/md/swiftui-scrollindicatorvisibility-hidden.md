

- SwiftUI
- ScrollIndicatorVisibility
-  hidden 

Type Property

# hidden

Hide the scroll indicators.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var hidden: ScrollIndicatorVisibility { get }
```

## Discussion

By default, scroll views in macOS show indicators when a mouse is connected. Use never to indicate a stronger preference that can override this behavior.

## See Also

### Getting visibilties

static var automatic: ScrollIndicatorVisibility

Scroll indicator visibility depends on the policies of the component accepting the visibility configuration.

static var never: ScrollIndicatorVisibility

Scroll indicators should never be visible.

static var visible: ScrollIndicatorVisibility

Show the scroll indicators.

