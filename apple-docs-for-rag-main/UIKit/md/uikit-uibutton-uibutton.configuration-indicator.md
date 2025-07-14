

- UIKit
- UIButton
- UIButton.Configuration
-  indicator 

Instance Property

# indicator

The style of the indicator that appears on the button.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
var indicator: UIButton.Configuration.Indicator { get set }
```

## Discussion

Use this property to control the style of the indicator that appears on the trailing edge of the button. For example, the following code disables the indicator by setting this style to UIButton.Configuration.Indicator.none.

```
var config = UIButton.Configuration.filled()
config.indicator = .none
```

## See Also

### Configuring the indicator

enum Indicator

Constants that determine the style of the indicator that appears on a button.

var indicatorColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the indicator color.

