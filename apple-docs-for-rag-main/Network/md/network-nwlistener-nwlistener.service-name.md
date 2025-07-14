

- Network
- NWListener
- NWListener.Service
-  name 

Instance Property

# name

The Bonjour name of the service.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
let name: String?
```

## See Also

### Inspecting Services

let type: String

The Bonjour type of the service.

let domain: String?

The Bonjour domain of the service.

var txtRecordObject: NWTXTRecord?

The TXT record to advertise with the service.

let txtRecord: Data?

The TXT record as a raw buffer to advertise with the service.

