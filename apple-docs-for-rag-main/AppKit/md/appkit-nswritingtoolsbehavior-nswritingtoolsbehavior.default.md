

- AppKit
- NSWritingToolsBehavior
-  NSWritingToolsBehavior.default 

Case

# NSWritingToolsBehavior.default

An option to let the system determine the best way to enable Writing Tools for the view.

macOS 15.0+

``` source
case `default`
```

## Discussion

The system chooses a complete, limited, or none experience based on the device-level support for the feature.

## See Also

### Getting the Writing Tools behaviors

case none

An option to prevent Writing Tools from modifying the text in the view.

case complete

An option to provide the complete Writing Tools experience for the text view.

case limited

An option to provide a limited, overlay-panel experience for the text view.

