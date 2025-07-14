

- UIKit
- UIButton
- UIButton.Configuration
-  cornerStyle 

Instance Property

# cornerStyle

The button style that controls the display behavior of the background corner radius.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var cornerStyle: UIButton.Configuration.CornerStyle { get set }
```

## Discussion

This property controls the behavior of the cornerRadius you set on the configuration background. The default corner style is UIButton.Configuration.CornerStyle.dynamic.

## See Also

### Configuring the button background

var background: UIBackgroundConfiguration

The configuration to customize the button background.

enum CornerStyle

Settings that determine the appearance of the background corner radius.

