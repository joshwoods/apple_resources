

- UIKit
- UITabBar
-  barStyle 

Instance Property

# barStyle

The tab bar style that specifies its appearance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var barStyle: UIBarStyle { get set }
```

## Discussion

This property determines whether the tab bar uses a dark or light visual style when no background image or tint color is specified. Together with the isTranslucent property, this property defines the default visual style of the tab bar. Set this property to the value that best matches the style of your interface. For a list of possible values, see UIBarStyle. The default value of this property is UIBarStyle.default.

## See Also

### Setting the bar’s style

enum UIBarStyle

Defines the stylistic appearance of different types of views.

