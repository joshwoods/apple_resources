

- IOBluetooth
- OBEXSession
-  obexSetPath(\_:constants:optionalHeaders:optionalHeadersLength:eventSelector:selectorTarget:refCon:) 

Instance Method

# obexSetPath(\_:constants:optionalHeaders:optionalHeadersLength:eventSelector:selectorTarget:refCon:)

Send an OBEX SetPath command to the session’s target.

macOS

``` source
func obexSetPath(
    _ inFlags: OBEXFlags,
    constants inConstants: OBEXConstants,
    optionalHeaders inOptionalHeaders: UnsafeMutableRawPointer!,
    optionalHeadersLength inOptionalHeadersLength: Int,
    eventSelector inSelector: Selector!,
    selectorTarget inTarget: Any!,
    refCon inUserRefCon: UnsafeMutableRawPointer!
) -> OBEXError
```

## Parameters 

`inFlags`  

OBEX setpath flags. See OBEX.h for possibilities.

`inConstants`  

OBEX setpath constants. See OBEX.h for possibilities.

`inOptionalHeaders`  

Can be NULL. Ptr to some data you want to send as your optional headers. Use the provided header contruction kit in OBEX.h and OBEXHeadersToBytes() for convenience.

`inOptionalHeadersLength`  

Length of data in ptr passed in above.

`inSelector`  

A VALID selector to be called when something interesting happens due to this call. Selector in your target object MUST have the following signature, or it will not be called properly (look for error messages in Console.app):

- (void)OBEXSetPathHandler:(const OBEXSessionEvent\*)inSessionEvent;

`inTarget`  

A VALID target object for the selector.

`inUserRefCon`  

Whatever you want to pass here. It will be passed back to you in the refCon portion of the OBEXSessionEvent struct. nil is, of course, OK here.

## Discussion

A NULL selector or target will result in an error. After return, the data passed in will have been sent over the transport. You will receive a response to your command on your selector.

