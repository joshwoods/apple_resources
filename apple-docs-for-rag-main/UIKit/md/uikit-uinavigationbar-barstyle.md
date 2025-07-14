

- UIKit
- UINavigationBar
-  barStyle 

Instance Property

# barStyle

The navigation bar style that specifies its appearance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var barStyle: UIBarStyle { get set }
```

## Discussion

See UIBarStyle for possible values. The default value is UIBarStyle.default.

It is permissible to set the value of this property when the navigation bar is being managed by a navigation controller object.

## See Also

### Setting the bar’s style

enum UIBarStyle

Defines the stylistic appearance of different types of views.

