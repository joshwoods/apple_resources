

- IOBluetooth
-  OBEXAddByteSequenceHeader(\_:\_:\_:) 

Function

# OBEXAddByteSequenceHeader(\_:\_:\_:)

Add a byte sequence header to a dictionary of OBEXheaders.

macOS

``` source
func OBEXAddByteSequenceHeader(
    _ inHeaderData: UnsafeRawPointer!,
    _ inHeaderDataLength: UInt32,
    _ dictRef: CFMutableDictionary!
) -> OBEXError
```

## Parameters 

`inHeaderData`  

Bytes you want to put in the byte sequence header.

`inHeaderDataLength`  

Length of the bytes you want to put in the byte sequence header.

`dictRef`  

Dictionary you have allocated to hold the headers. Make sure it’s mutable.

## Return Value

Error code, kOBEXSuccess (0) if success.

## Discussion

Byte Sequence header - OBEX Spec, 2.2.5: Byte sequence. One thing of important note here - since we don’t know what Header Identifier and length you intend to use here, you MUST include your own identifier and length in the data you pass. Thus, your data must be in this format: \\\ Also, note that LENGTH = (3 + n), (1 for HI, 2 for the 2 bytes of length information, plus your n bytes of custom data). Be careful here to not mess up these values, as it could adversely affect the ability of the remote-device’s headers parser.

## See Also

### Miscellaneous

func OBEXAddApplicationParameterHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes representing an application parameter to a dictionary of OBEX headers.

func OBEXAddAuthorizationChallengeHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an authorization challenge header to a dictionary of OBEXheaders.

func OBEXAddAuthorizationResponseHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an authorization Response header to a dictionary of OBEXheaders.

func OBEXAddBodyHeader(UnsafeRawPointer!, UInt32, Bool, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddConnectionIDHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes representing a connection ID to a dictionary of OBEX headers.

func OBEXAddCountHeader(UInt32, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddDescriptionHeader(CFString!, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddHTTPHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddLengthHeader(UInt32, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddNameHeader(CFString!, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddObjectClassHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an object class header to a dictionary of OBEXheaders.

func OBEXAddTargetHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddTime4ByteHeader(UInt32, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

func OBEXAddTimeISOHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes to a dictionary of OBEXheaders.

func OBEXAddTypeHeader(CFString!, CFMutableDictionary!) -> OBEXError

Add a CFStringRef to a dictionary of OBEXheaders.

