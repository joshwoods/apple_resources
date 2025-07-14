

- Multipeer Connectivity
- MCNearbyServiceBrowser
-  init(peer:serviceType:) 

Initializer

# init(peer:serviceType:)

Initializes the nearby service browser object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
init(
    peer myPeerID: MCPeerID,
    serviceType: String
)
```

## Parameters 

`myPeerID`  

The local peer ID for this instance.

`serviceType`  

The type of service to search for. This should be a *short* text string that describes the app’s networking protocol, in the same format as a Bonjour service type (without the transport protocol) and meeting the restrictions of RFC 6335 (section 5.1) governing Service Name Syntax. In particular, the string:

- Must be 1–15 characters long

- Can contain only ASCII lowercase letters, numbers, and hyphens

- Must contain at least one ASCII letter

- Must not begin or end with a hyphen

- Must not contain hyphens adjacent to other hyphens.

This name should be easily distinguished from unrelated services. For example, a text chat app made by ABC company could use the service type `abc-txtchat`.

For more details, read Domain Naming Conventions.

## Return Value

Returns an initialized nearby service browser object, or `nil` if an error occurs.

## Discussion

This method throws an exception if the `session` or `serviceType` parameters do not contain valid objects or the specified Bonjour service type is not valid.

## See Also

### Initializing the Browser

var delegate: (any MCNearbyServiceBrowserDelegate)?

The delegate object that handles browser-related events.

var myPeerID: MCPeerID

The local peer ID for this instance.

var serviceType: String

The service type to browse for.

