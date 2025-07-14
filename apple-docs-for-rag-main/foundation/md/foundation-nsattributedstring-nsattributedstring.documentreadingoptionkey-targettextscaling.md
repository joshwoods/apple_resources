

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  targetTextScaling 

Type Property

# targetTextScaling

The text scaling mode to use after reading the text from disk.

FoundationUIKitiOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let targetTextScaling: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

The value of this property is one of the options of the NSTextScalingType type. Some platforms scale fonts to improve their appearance. Include this option to specify the text-scaling mode you want to use for the document you read.

## See Also

### Getting the font-scaling options

static let sourceTextScaling: NSAttributedString.DocumentReadingOptionKey

The text-scaling mode to associate with the document’s content.

