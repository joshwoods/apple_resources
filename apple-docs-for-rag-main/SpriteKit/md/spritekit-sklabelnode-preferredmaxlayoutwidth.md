

- SpriteKit
- SKLabelNode
-  preferredMaxLayoutWidth 

Instance Property

# preferredMaxLayoutWidth

The width, in screen points, after which line-break mode should be applied.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

**watchOS**

``` source
var preferredMaxLayoutWidth: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var preferredMaxLayoutWidth: CGFloat { get set }
```

## Discussion

The default value is 0, which means that line break mode will not be applied.

## See Also

### Defining a Label’s Line-Breaking Behavior

var lineBreakMode: NSLineBreakMode

Determines the line-break mode for multiple lines.

var numberOfLines: Int

Determines the number of lines to draw.

