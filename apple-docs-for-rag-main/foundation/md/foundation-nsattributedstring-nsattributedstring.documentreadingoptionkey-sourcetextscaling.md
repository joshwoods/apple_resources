

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  sourceTextScaling 

Type Property

# sourceTextScaling

The text-scaling mode to associate with the document’s content.

FoundationUIKitiOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let sourceTextScaling: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

The value of this property is one of the options of the NSTextScalingType type. Some platforms scale fonts to improve their appearance. Include this option to specify the text-scaling mode to associate with the document’s contents on disk.

## See Also

### Getting the font-scaling options

static let targetTextScaling: NSAttributedString.DocumentReadingOptionKey

The text scaling mode to use after reading the text from disk.

