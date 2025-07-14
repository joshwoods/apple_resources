

- AppKit
- NSTextTab
-  init(type:location:) 

Initializer

# init(type:location:)

Initializes a newly allocated text tab with the specified alignment and location.

macOS

``` source
convenience init(
    type: NSParagraphStyle.TextTabType,
    location loc: CGFloat
)
```

## Discussion

The location is relative to the back margin, based on the line sweep direction of the paragraph. The value in the `type` parameter can be any of the values described in NSParagraphStyle.TextTabType.

## See Also

### Deprecated

var tabStopType: NSParagraphStyle.TextTabType

The text tab’s type of tab stop.

