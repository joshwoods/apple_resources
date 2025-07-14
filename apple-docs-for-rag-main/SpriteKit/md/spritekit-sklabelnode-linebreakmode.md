

- SpriteKit
- SKLabelNode
-  lineBreakMode 

Instance Property

# lineBreakMode

Determines the line-break mode for multiple lines.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var lineBreakMode: NSLineBreakMode { get set }
```

**watchOS**

``` source
var lineBreakMode: NSLineBreakMode { get set }
```

## Discussion

The default value is NSLineBreakByTruncatingTail.

## See Also

### Defining a Label’s Line-Breaking Behavior

var preferredMaxLayoutWidth: CGFloat

The width, in screen points, after which line-break mode should be applied.

var numberOfLines: Int

Determines the number of lines to draw.

