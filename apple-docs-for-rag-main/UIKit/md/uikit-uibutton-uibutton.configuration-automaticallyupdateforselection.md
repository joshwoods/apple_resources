

- UIKit
- UIButton
- UIButton.Configuration
-  automaticallyUpdateForSelection 

Instance Property

# automaticallyUpdateForSelection

A Boolean value that determines whether the style automatically updates when the button is in a selected state.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var automaticallyUpdateForSelection: Bool { get set }
```

## Discussion

The default value is true for the plain(), gray(), and tinted() configurations. Set this value to false to customize the selection behavior.

