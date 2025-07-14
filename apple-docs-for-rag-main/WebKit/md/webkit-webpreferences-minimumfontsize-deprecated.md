

- WebKit
- WebPreferences
-  minimumFontSize Deprecated

Instance Property

# minimumFontSize

The minimum font size of the web view.

macOS 10.3–10.14Deprecated

``` source
var minimumFontSize: Int32 { get set }
```

## Discussion

This sets the minimum display font size for the web view, overriding all content-specified styles, including explicitly specified font sizes.

The font size specified by `size` should always be greater than zero.

## See Also

### Getting and Setting Font Sizes

var defaultFixedFontSize: Int32

The default fixed font size of the web view.

Deprecated

var defaultFontSize: Int32

The default font size of the web view.

Deprecated

var minimumLogicalFontSize: Int32

The minimum logical font size of the web view.

Deprecated

