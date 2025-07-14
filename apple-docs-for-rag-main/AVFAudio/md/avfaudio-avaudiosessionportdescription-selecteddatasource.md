

- AVFAudio
- AVAudioSessionPortDescription
-  selectedDataSource 

Instance Property

# selectedDataSource

The currently selected audio data source for the port.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var selectedDataSource: AVAudioSessionDataSourceDescription? { get }
```

## Discussion

If this property returns `nil`, the port doesn’t support selecting between multiple data sources.

## See Also

### Managing a Port’s Data Sources

var dataSources: [AVAudioSessionDataSourceDescription]?

The available data sources for the port.

var preferredDataSource: AVAudioSessionDataSourceDescription?

The preferred audio data source for the port.

func setPreferredDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the preferred audio data source for the port.

