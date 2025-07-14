

- External Accessory
- EASession
-  init(accessory:forProtocol:) 

Initializer

# init(accessory:forProtocol:)

Initializes the session for the specified accessory and protocol.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
init?(
    accessory: EAAccessory,
    forProtocol protocolString: String
)
```

## Parameters 

`accessory`  

The accessory with which you want to communicate. You can get a list of accessory objects from the EAAccessoryManager object.

`protocolString`  

The protocol to use when communicating with the accessory. This protocol must be one that the accessory understands. All communications with the accessory are expected to use this protocol.

## Return Value

The initialized session object. This method may return `nil` if the accessory does not recognize the specified protocol or there was an error communicating with the accessory.

## Discussion

There can be only one session object at a time for a given accessory and protocol combination.

