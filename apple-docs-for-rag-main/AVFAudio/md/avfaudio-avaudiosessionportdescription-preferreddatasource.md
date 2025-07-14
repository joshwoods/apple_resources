

- AVFAudio
- AVAudioSessionPortDescription
-  preferredDataSource 

Instance Property

# preferredDataSource

The preferred audio data source for the port.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredDataSource: AVAudioSessionDataSourceDescription? { get }
```

## Discussion

The value of this property indicates the data source selected using the setPreferredDataSource(_:) method. To see the actual data source, use the selectedDataSource property.

If `nil`, the port doesn’t support selecting between multiple data sources, or no preferred data source has been selected.

## See Also

### Managing a Port’s Data Sources

var dataSources: [AVAudioSessionDataSourceDescription]?

The available data sources for the port.

var selectedDataSource: AVAudioSessionDataSourceDescription?

The currently selected audio data source for the port.

func setPreferredDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the preferred audio data source for the port.

