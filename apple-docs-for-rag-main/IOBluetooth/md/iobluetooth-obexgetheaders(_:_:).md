

- IOBluetooth
-  OBEXGetHeaders(\_:\_:) 

Function

# OBEXGetHeaders(\_:\_:)

Take a data blob and looks for OBEX headers.

macOS

``` source
func OBEXGetHeaders(
    _ inData: UnsafeRawPointer!,
    _ inDataSize: Int
) -> CFDictionary!
```

## Parameters 

`inData`  

The data chunk with the headers you are interested in.

`inDataSize`  

The size of the buffer you are passing in.

## Return Value

A CFDictionary with the headers found in the data blob inside it.

## Discussion

You should use this when your callback for PUTs, GETs, etc. give you a data chunk and a size. Pass these params to this function and you will receive a dictionary back full of the parse headers. You can use the CFDictionary calls to get objects out of it, based on the header keys defined above. You are responsible for releasing the CFDictionary returned to you. Example usage:

```
```

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

