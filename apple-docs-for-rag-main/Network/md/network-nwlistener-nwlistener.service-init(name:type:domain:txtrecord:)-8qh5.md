

- Network
- NWListener
- NWListener.Service
-  init(name:type:domain:txtRecord:) 

Initializer

# init(name:type:domain:txtRecord:)

Initializes a Bonjour service to advertise with a TXT record.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    name: String? = nil,
    type: String,
    domain: String? = nil,
    txtRecord: NWTXTRecord
)
```

## Discussion

Advertised services are primarily defined by their types. If you do not specify a service name, the device name will be chosen. You should not specify a Bonjour domain unless you know you need to advertise only on a particular domain.

## See Also

### Defining Services

init(name: String?, type: String, domain: String?, txtRecord: Data?)

Initializes a Bonjour service to advertise.

var noAutoRename: Bool

A Boolean that indicates whether the service prohibits automatic renaming in the event of a name conflict.

