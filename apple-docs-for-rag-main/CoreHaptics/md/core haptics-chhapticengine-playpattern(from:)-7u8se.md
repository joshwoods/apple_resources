

- Core Haptics
- CHHapticEngine
-  playPattern(from:) 

Instance Method

# playPattern(from:)

Plays a pattern from the specified data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func playPattern(from data: Data) throws
```

## Parameters 

`data`  

The raw data containing the haptic pattern, structured as an AHAP dictionary.

## Discussion

Start the engine prior to calling this method to provide low-latency playback. If the engine isn’t already running when you call this method, the system starts it, which can result in a significant playback delay.

## See Also

### Playing a Pattern

func playPattern(from: URL) throws

Plays a pattern that’s defined in a file at the specified URL.

