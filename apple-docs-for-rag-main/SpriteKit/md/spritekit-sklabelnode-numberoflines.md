

- SpriteKit
- SKLabelNode
-  numberOfLines 

Instance Property

# numberOfLines

Determines the number of lines to draw.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

**watchOS**

``` source
var numberOfLines: Int { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var numberOfLines: Int { get set }
```

## Discussion

The default value is 1 (a single line). A value of 0 in interpreted as an unlimited number of lines. If the height of the text reaches the number of lines, the text will be truncated using the line break mode.

## See Also

### Defining a Label’s Line-Breaking Behavior

var preferredMaxLayoutWidth: CGFloat

The width, in screen points, after which line-break mode should be applied.

var lineBreakMode: NSLineBreakMode

Determines the line-break mode for multiple lines.

