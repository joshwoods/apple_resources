

- UIKit
- UIButton
- UIButton.Configuration
-  macIdiomStyle 

Instance Property

# macIdiomStyle

The style to use when this button appears in macOS.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var macIdiomStyle: UIButton.Configuration.MacIdiomStyle { get set }
```

## Discussion

Use this property when building your app with Mac Catalyst. The value UIButton.Configuration.MacIdiomStyle.automatic lets the system choose the appropriate style. Select a specific style to force the button to always use that style.

## See Also

### Configuring the appearance on macOS

enum MacIdiomStyle

The button style your app uses when running in macOS.

