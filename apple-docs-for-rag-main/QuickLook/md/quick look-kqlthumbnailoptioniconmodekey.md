

- Quick Look
-  kQLThumbnailOptionIconModeKey 

Global Variable

# kQLThumbnailOptionIconModeKey

The Quick Look generator produces the thumbnail as an icon with decor.

macOS 10.5+

``` source
let kQLThumbnailOptionIconModeKey: CFString!
```

## Discussion

The default value is kCFBooleanFalse. If you use the default, the Quick Look feature creates a thumbnail image with no icon decor. To create the thumbnail as an icon, set the value to kCFBooleanTrue. The icon’s image includes all the typical icon decor, such as shadows and a curled corner.

## See Also

### Constants

var kQLReturnMask: Int32

The Quick Look generator can create a preview.

var kQLReturnHasMore: Int32

The Quick Look generator has more content to display as part of the preview.

let kQLThumbnailOptionScaleFactorKey: CFString!

The scale factor for the thumbnail.

var QUICKLOOK_VERSION: Int32

