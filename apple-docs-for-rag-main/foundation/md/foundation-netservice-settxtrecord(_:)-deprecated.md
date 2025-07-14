

- Foundation
- NetService
-  setTXTRecord(\_:) Deprecated

Instance Method

# setTXTRecord(\_:)

Sets the TXT record for the receiver, and returns a Boolean value that indicates whether the operation was successful.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func setTXTRecord(_ recordData: Data?) -> Bool
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Parameters 

`recordData`  

The TXT record for the receiver.

## Return Value

true if `recordData` is successfully set as the TXT record, otherwise false.

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

var delegate: (any NetServiceDelegate)?

The delegate for the receiver.

Deprecated

