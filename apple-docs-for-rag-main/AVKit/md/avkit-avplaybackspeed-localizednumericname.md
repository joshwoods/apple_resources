

- AVKit
- AVPlaybackSpeed
-  localizedNumericName 

Instance Property

# localizedNumericName

A localized numeric name for a speed that’s suitable for display in a user interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var localizedNumericName: String { get }
```

## Discussion

Use this value to represent the speed in a user interface where limited space is available. Represent the speed using its localizedName value where space allows.

## See Also

### Inspecting Speed Details

var rate: Float

The playback rate to use when you select this speed.

var localizedName: String

A localized name for a speed that’s suitable for display in a user interface.

