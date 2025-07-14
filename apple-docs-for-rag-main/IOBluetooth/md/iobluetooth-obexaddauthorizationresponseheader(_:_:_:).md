

- IOBluetooth
-  OBEXAddAuthorizationResponseHeader(\_:\_:\_:) 

Function

# OBEXAddAuthorizationResponseHeader(\_:\_:\_:)

Add an authorization Response header to a dictionary of OBEXheaders.

macOS

``` source
func OBEXAddAuthorizationResponseHeader(
    _ inHeaderData: UnsafeRawPointer!,
    _ inHeaderDataLength: UInt32,
    _ dictRef: CFMutableDictionary!
) -> OBEXError
```

## Parameters 

`inHeaderData`  

Bytes you want to put in the authorization Response header.

`inHeaderDataLength`  

Length of the bytes you want to put in authorization Response header.

`dictRef`  

Dictionary you have allocated to hold the headers. Make sure it’s mutable.

## Return Value

Error code, kOBEXSuccess (0) if success.

## Discussion

Authorization Response header - OBEX Spec, 2.2.14: Authorization Response.

## See Also

### Miscellaneous

func OBEXAddApplicationParameterHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add bytes representing an application parameter to a dictionary of OBEX headers.

func OBEXAddAuthorizationChallengeHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add an authorization challenge header to a dictionary of OBEXheaders.

func OBEXAddBodyHeader(UnsafeRawPointer!, UInt32, Bool, CFMutableDictionary!) -> OBEXError

Add bytes of data to a dictionary of OBEXheaders.

func OBEXAddByteSequenceHeader(UnsafeRawPointer!, UInt32, CFMutableDictionary!) -> OBEXError

Add a byte sequence header to a dictionary of OBEXheaders.

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

