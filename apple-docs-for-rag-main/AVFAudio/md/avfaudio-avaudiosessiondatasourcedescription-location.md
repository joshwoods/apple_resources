

- AVFAudio
- AVAudioSessionDataSourceDescription
-  location 

Instance Property

# location

The location of the data source on the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var location: AVAudioSession.Location? { get }
```

## Discussion

This property returns `nil` if the data source’s location isn’t known.

## See Also

### Retrieving the Data Source Location

struct Location

Constants that describe the location of the data source on device.

