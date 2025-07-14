

- UIKit
- UIWritingToolsBehavior
-  UIWritingToolsBehavior.default 

Case

# UIWritingToolsBehavior.default

An option to let the system determine the best way to enable writing tools for the view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
case `default`
```

## Discussion

The system chooses a complete, limited, or none experience based on the device-level support for the feature.

## See Also

### Getting the writing tools behaviors

case none

An option to prevent the writing tools from modifying the text in the view.

case complete

An option to provide the complete writing tools experience for the text view.

case limited

An option to provide a limited, overlay-panel experience for the text view.

