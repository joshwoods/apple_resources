

- AVKit
- AVPlaybackSpeed
-  localizedName 

Instance Property

# localizedName

A localized name for a speed that’s suitable for display in a user interface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var localizedName: String { get }
```

## Discussion

Use this value to represent the speed in a user interface where space allows. Use the localizedNumericName where limited space is available.

## See Also

### Inspecting Speed Details

var rate: Float

The playback rate to use when you select this speed.

var localizedNumericName: String

A localized numeric name for a speed that’s suitable for display in a user interface.

