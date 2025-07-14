

- AVFAudio
- AVAudioSessionPortDescription
-  dataSources 

Instance Property

# dataSources

The available data sources for the port.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var dataSources: [AVAudioSessionDataSourceDescription]? { get }
```

## Discussion

This feature is only supported on certain devices and peripherals; for example, the data sources represent front- and rear-facing microphones on a device.

Some, but not all, USB ports provide a set of data sources. For example, a USB audio interface may allow you to select between a built-in microphone or external microphone input. The output side may allow you to select between headphones or externally powered speakers. The audio session interface represents the input and output sides of the USB interface as two separate ports of type usbAudio.

If this property is `nil`, the port doesn’t support selecting between multiple data sources.

The contents of this array may change if you change the audio session’s mode.

## See Also

### Managing a Port’s Data Sources

var selectedDataSource: AVAudioSessionDataSourceDescription?

The currently selected audio data source for the port.

var preferredDataSource: AVAudioSessionDataSourceDescription?

The preferred audio data source for the port.

func setPreferredDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the preferred audio data source for the port.

