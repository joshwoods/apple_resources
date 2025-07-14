

- Foundation
- NetService
-  addresses Deprecated

Instance Property

# addresses

A read-only array containing `NSData` objects, each of which contains a socket address for the service.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
var addresses: [Data]? { get }
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Discussion

An array containing `NSData` objects, each of which contains a socket address for the service. Each `NSData` object in the returned array contains an appropriate `sockaddr` structure that you can use to connect to the socket. The exact type of this structure depends on the service to which you are connecting. If no addresses were resolved for the service, the returned array contains zero elements.

It is possible for a single service to resolve to more than one address or not resolve to any addresses. A service might resolve to multiple addresses if the computer publishing the service is currently multihoming.

Backward Compatibility Note

This became a property in OS X v10.9 and iOS 7, but the underlying getter method (`addresses`) has been available since this class was first introduced.

## See Also

### Related Documentation

func resolve()

Starts a resolve process for the service.

Deprecated

### Configuring Network Services

class func data(fromTXTRecord: [String : Data]) -> Data

Returns an `NSData` object representing a TXT record formed from a given dictionary.

Deprecated

class func dictionary(fromTXTRecord: Data) -> [String : Data]

Returns a dictionary representing a TXT record given as an `NSData` object.

Deprecated

var domain: String

A string containing the domain for this service.

Deprecated

var includesPeerToPeer: Bool

Specifies whether to also publish, resolve, or monitor this service over peer-to-peer Bluetooth and Wi-Fi, if available. false by default.

func getInputStream(UnsafeMutablePointer&lt;InputStream?>?, outputStream: UnsafeMutablePointer&lt;OutputStream?>?) -> Bool

Creates a pair of input and output streams for the receiver and returns a Boolean value that indicates whether they were retrieved successfully.

Deprecated

var name: String

A string containing the name of this service.

Deprecated

var type: String

The type of the published service.

Deprecated

func txtRecordData() -> Data?

Returns the TXT record for the receiver.

Deprecated

func setTXTRecord(Data?) -> Bool

Sets the TXT record for the receiver, and returns a Boolean value that indicates whether the operation was successful.

Deprecated

var delegate: (any NetServiceDelegate)?

The delegate for the receiver.

Deprecated

