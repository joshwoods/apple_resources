

- Foundation
- NSAttributedString
- NSAttributedString.DocumentAttributeKey
-  textScaling 

Type Property

# textScaling

The text-scaling mode to use when displaying the text.

FoundationUIKitiOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let textScaling: NSAttributedString.DocumentAttributeKey
```

## Discussion

The value of this property is one of the options of the NSTextScalingType type. Some platforms scale fonts to improve their appearance. When saving a document, include this attribute to specify the type of scaling to apply to the text at display time.

## See Also

### Getting the font-scaling options

static let sourceTextScaling: NSAttributedString.DocumentAttributeKey

The text-scaling mode you used when creating the text.

