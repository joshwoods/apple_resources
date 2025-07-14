

- Quick Look
-  kQLThumbnailOptionScaleFactorKey 

Global Variable

# kQLThumbnailOptionScaleFactorKey

The scale factor for the thumbnail.

macOS 10.5+

``` source
let kQLThumbnailOptionScaleFactorKey: CFString!
```

## Discussion

The scale factor is a `float` value that’s encapsulated in a doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd object. If this option is absent, the default value is `1.0`.

## See Also

### Constants

var kQLReturnMask: Int32

The Quick Look generator can create a preview.

var kQLReturnHasMore: Int32

The Quick Look generator has more content to display as part of the preview.

let kQLThumbnailOptionIconModeKey: CFString!

The Quick Look generator produces the thumbnail as an icon with decor.

var QUICKLOOK_VERSION: Int32

