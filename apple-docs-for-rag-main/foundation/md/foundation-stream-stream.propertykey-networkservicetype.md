

- Foundation
- Stream
- Stream.PropertyKey
-  networkServiceType 

Type Property

# networkServiceType

The type of service for the stream. Providing the service type allows the system to properly handle certain attributes of the stream, including routing and suspension behavior. Most streams do not need to set this property. See `Stream Service Types` for a list of possible values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let networkServiceType: Stream.PropertyKey
```

## See Also

### Type Properties

static let dataWrittenToMemoryStreamKey: Stream.PropertyKey

Value is an `NSData` instance containing the data written to a memory stream.

static let fileCurrentOffsetKey: Stream.PropertyKey

Value is an `NSNumber` object containing the current absolute offset of the stream.

static let socketSecurityLevelKey: Stream.PropertyKey

static let socksProxyConfigurationKey: Stream.PropertyKey

Value is an `NSDictionary` object containing SOCKS proxy configuration information.

