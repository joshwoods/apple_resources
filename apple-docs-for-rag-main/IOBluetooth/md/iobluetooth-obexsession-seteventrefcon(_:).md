

- IOBluetooth
- OBEXSession
-  setEventRefCon(\_:) 

Instance Method

# setEventRefCon(\_:)

Sets the C-API callback refCon used when the session recieves data.

macOS

``` source
func setEventRefCon(_ inRefCon: UnsafeMutableRawPointer!)
```

## Parameters 

`inRefCon`  

User’s refCon that will get passed when their event callback is invoked.

## Discussion

This is really not intended for client sessions. Only subclasses would really be interested in using this. They should set these when their subclass object is created, because otherwise they will have no context in their callback.

