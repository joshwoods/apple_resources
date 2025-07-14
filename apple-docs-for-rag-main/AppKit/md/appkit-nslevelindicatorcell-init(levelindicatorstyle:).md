

- AppKit
- NSLevelIndicatorCell
-  init(levelIndicatorStyle:) 

Initializer

# init(levelIndicatorStyle:)

Initializes the receiver with the style specified by `levelIndicatorStyle`.

macOS

``` source
@MainActor
init(levelIndicatorStyle: NSLevelIndicator.Style)
```

## Discussion

The default value and minimum value are `0.0`. The default maximum value is dependent on `levelIndicatorStyle`. For continuous styles, the default maximum value is `100.0`. For discrete styles, the default maximum value is `5.0`.

