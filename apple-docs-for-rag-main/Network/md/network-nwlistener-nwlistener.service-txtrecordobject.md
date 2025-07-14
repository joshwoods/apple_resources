

- Network
- NWListener
- NWListener.Service
-  txtRecordObject 

Instance Property

# txtRecordObject

The TXT record to advertise with the service.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var txtRecordObject: NWTXTRecord? { get set }
```

## See Also

### Inspecting Services

let name: String?

The Bonjour name of the service.

let type: String

The Bonjour type of the service.

let domain: String?

The Bonjour domain of the service.

let txtRecord: Data?

The TXT record as a raw buffer to advertise with the service.

