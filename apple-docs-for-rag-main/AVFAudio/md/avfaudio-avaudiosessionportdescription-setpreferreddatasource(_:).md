

- AVFAudio
- AVAudioSessionPortDescription
-  setPreferredDataSource(\_:) 

Instance Method

# setPreferredDataSource(\_:)

Sets the preferred audio data source for the port.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setPreferredDataSource(_ dataSource: AVAudioSessionDataSourceDescription?) throws
```

## Parameters 

`dataSource`  

The data source to use.

## Discussion

Call this method to request a change to the audio session’s preferred data source. To determine whether the change has taken effect, inspect the selectedDataSource property. (For details, see Configuring standard audio behaviors in the AVAudioSession class reference).

If the port is in use, changing this setting is likely to result in a route reconfiguration.

Set a preferred data source only after setting the audio session’s category and mode, and activating the session.

## See Also

### Managing a Port’s Data Sources

var dataSources: [AVAudioSessionDataSourceDescription]?

The available data sources for the port.

var selectedDataSource: AVAudioSessionDataSourceDescription?

The currently selected audio data source for the port.

var preferredDataSource: AVAudioSessionDataSourceDescription?

The preferred audio data source for the port.

