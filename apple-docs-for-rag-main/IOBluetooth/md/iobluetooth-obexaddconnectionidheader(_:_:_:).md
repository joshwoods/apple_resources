

- IOBluetooth
-  OBEXAddConnectionIDHeader(\_:\_:\_:) 

Function

# OBEXAddConnectionIDHeader(\_:\_:\_:)

Add bytes representing a connection ID to a dictionary of OBEX headers.

macOS

``` source
func OBEXAddConnectionIDHeader(
    _ inHeaderData: UnsafeRawPointer!,
    _ inHeaderDataLength: UInt32,
    _ dictRef: CFMutableDictionary!
) -> OBEXError
```

## Parameters 

`inHeaderData`  

Connection ID data. Should be 4 bytes in length only.

`inHeaderDataLength`  

Length of Connection ID data. This should ONLY be set to equal 4.

`dictRef`  

Dictionary you have allocated to hold the headers. Make sure it’s mutable.

## Return Value

Error code, kOBEXSuccess (0) if success.

## Discussion

ConnectionID headers - OBEX Spec, 2.2.10: Byte Sequence

\*\*\* IMPORTANT NOTE: In bluetooth 1.0, using this function will allow you to pass in any value. You should not pass more than 4 bytes ever. In later releases, if the length passed is not 4, a kOBEXBadArgumentError error will be returned. \*\*\*

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

func OBEXAddByteSequenceHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add a byte sequence header to a dictionary of OBEXheaders.

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

