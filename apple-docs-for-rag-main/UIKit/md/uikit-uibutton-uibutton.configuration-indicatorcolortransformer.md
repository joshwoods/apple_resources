

- UIKit
- UIButton
- UIButton.Configuration
-  indicatorColorTransformer 

Instance Property

# indicatorColorTransformer

The color transformer for resolving the indicator color.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
var indicatorColorTransformer: UIConfigurationColorTransformer? { get set }
```

## Discussion

Use this color transformer to set a custom color for indicator. For example, the following code uses a grayscale color for the indicator instead of the default color.

```
var config = UIButton.Configuration.filled()
config.indicatorColorTransformer = UIConfigurationColorTransformer.grayscale
```

## See Also

### Configuring the indicator

var indicator: UIButton.Configuration.Indicator

The style of the indicator that appears on the button.

enum Indicator

Constants that determine the style of the indicator that appears on a button.

