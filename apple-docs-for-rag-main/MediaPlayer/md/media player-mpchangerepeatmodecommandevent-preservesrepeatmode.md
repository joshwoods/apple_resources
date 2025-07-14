

- Media Player
- MPChangeRepeatModeCommandEvent
-  preservesRepeatMode 

Instance Property

# preservesRepeatMode

A Boolean value that indicates whether the chosen repeat mode is preserved between playback sessions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 8.0+visionOS 1.0+watchOS 5.0+

``` source
var preservesRepeatMode: Bool { get }
```

## Discussion

When set to true, the chosen repeat mode is preserved between playback sessions.

## See Also

### Changing the repeat type

var repeatType: MPRepeatType

The repeat type used when fulfilling the event request.

