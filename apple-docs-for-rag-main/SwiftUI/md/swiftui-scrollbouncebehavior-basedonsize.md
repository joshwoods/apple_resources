

- SwiftUI
- ScrollBounceBehavior
-  basedOnSize 

Type Property

# basedOnSize

The scrollable view bounces when its content is large enough to require scrolling.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
static var basedOnSize: ScrollBounceBehavior { get }
```

## Discussion

The scrollable view bounces along the specified axis if the size of the content exceeeds the size of the scrollable view in that axis.

## See Also

### Bounce behaviors

static var automatic: ScrollBounceBehavior

The automatic behavior.

static var always: ScrollBounceBehavior

The scrollable view always bounces.

