

- Foundation
- Stream
- Stream.PropertyKey
-  dataWrittenToMemoryStreamKey 

Type Property

# dataWrittenToMemoryStreamKey

Value is an `NSData` instance containing the data written to a memory stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let dataWrittenToMemoryStreamKey: Stream.PropertyKey
```

## Discussion

Use this property when you have an output-stream object instantiated to collect written data in memory. The value of this property is read-only.

## See Also

### Type Properties

static let fileCurrentOffsetKey: Stream.PropertyKey

Value is an `NSNumber` object containing the current absolute offset of the stream.

static let networkServiceType: Stream.PropertyKey

The type of service for the stream. Providing the service type allows the system to properly handle certain attributes of the stream, including routing and suspension behavior. Most streams do not need to set this property. See `Stream Service Types` for a list of possible values.

static let socketSecurityLevelKey: Stream.PropertyKey

static let socksProxyConfigurationKey: Stream.PropertyKey

Value is an `NSDictionary` object containing SOCKS proxy configuration information.

