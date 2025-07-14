

- Foundation
- NetService
-  domain Deprecated

Instance Property

# domain

A string containing the domain for this service.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
var domain: String { get }
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Discussion

This can be an explicit domain name or it can contain the generic local domain name, `@"local."` (note the trailing period, which indicates an absolute name).

This property’s value is set when the object is first initialized, whether by your code or by a browser object. See init(domain:type:name:) for more information.

Backward Compatibility Note

This became a property in OS X v10.9 and iOS 7, but the underlying getter method (`domain`) has been available since this class was first introduced.

## See Also

### Configuring Network Services

class func data(fromTXTRecord: [String : Data]) -> Data

Returns an `NSData` object representing a TXT record formed from a given dictionary.

Deprecated

class func dictionary(fromTXTRecord: Data) -> [String : Data]

Returns a dictionary representing a TXT record given as an `NSData` object.

Deprecated

var addresses: [Data]?

A read-only array containing `NSData` objects, each of which contains a socket address for the service.

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

