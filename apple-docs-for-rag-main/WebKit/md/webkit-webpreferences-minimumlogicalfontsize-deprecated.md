

- WebKit
- WebPreferences
-  minimumLogicalFontSize Deprecated

Instance Property

# minimumLogicalFontSize

The minimum logical font size of the web view.

macOS 10.3–10.14Deprecated

``` source
var minimumLogicalFontSize: Int32 { get set }
```

## Discussion

The minimum logical font size is the smallest font size that will display in a web view when the content’s font size is imprecisely specified. This includes content with logical sizes (such as `small`) or with a font size specified as a percentage of the default.

Most clients will not want to use this ; rather, explicitly set the minimum display font size using the minimumFontSize property.

The font size specified by `size` should always be greater than zero.

## See Also

### Getting and Setting Font Sizes

var defaultFixedFontSize: Int32

The default fixed font size of the web view.

Deprecated

var defaultFontSize: Int32

The default font size of the web view.

Deprecated

var minimumFontSize: Int32

The minimum font size of the web view.

Deprecated

