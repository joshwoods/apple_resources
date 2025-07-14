

- AVFAudio
- AVAudioSessionDataSourceDescription
-  dataSourceID 

Instance Property

# dataSourceID

The system-assigned identifier for the data source.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dataSourceID: NSNumber { get }
```

## Discussion

You can use the value of this property to assign a specific data source to some input or output within an audio session.

## See Also

### Identifying a Data Source

var dataSourceName: String

A human-readable name for the data source.

