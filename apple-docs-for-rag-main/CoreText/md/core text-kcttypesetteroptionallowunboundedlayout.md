

- Core Text
-  kCTTypesetterOptionAllowUnboundedLayout 

Global Variable

# kCTTypesetterOptionAllowUnboundedLayout

A key that specifies whether the text system lays out text that requires unreasonable effort.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
let kCTTypesetterOptionAllowUnboundedLayout: CFString
```

## Discussion

Proper Unicode layout of some text requires unreasonable effort. By default, the text system avoids expending this effort. To create a typesetter that always typesets the text, regardless of the amount of work needed, call CTTypesetterCreateWithAttributedStringAndOptions(_:_:) and set this option to kCFBooleanTrue.

The value for this key must be a `CFBooleanRef`. The default value is kCFBooleanFalse.

## See Also

### Constants

let kCTTypesetterOptionForcedEmbeddingLevel: CFString

A key that specifies the embedding level of the typesetter’s text.

let kCTTypesetterOptionDisableBidiProcessing: CFStringDeprecated

