

- Network
- NWListener
- NWListener.Service
-  init(name:type:domain:txtRecord:) 

Initializer

# init(name:type:domain:txtRecord:)

Initializes a Bonjour service to advertise.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init(
    name: String? = nil,
    type: String,
    domain: String? = nil,
    txtRecord: Data? = nil
)
```

## Discussion

Advertised services are primarily defined by their types. If you do not specify a service name, the device name will be chosen. You should not specify a Bonjour domain unless you know you need to advertise only on a particular domain.

## See Also

### Defining Services

init(name: String?, type: String, domain: String?, txtRecord: NWTXTRecord)

Initializes a Bonjour service to advertise with a TXT record.

var noAutoRename: Bool

A Boolean that indicates whether the service prohibits automatic renaming in the event of a name conflict.

