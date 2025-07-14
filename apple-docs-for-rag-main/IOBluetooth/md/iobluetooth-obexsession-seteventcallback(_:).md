

- IOBluetooth
- OBEXSession
-  setEventCallback(\_:) 

Instance Method

# setEventCallback(\_:)

Sets the C-API callback used when the session recieves data.

macOS

``` source
func setEventCallback(_ inEventCallback: OBEXSessionEventCallback!)
```

## Parameters 

`inEventCallback`  

Function to callback. Should be non-NULL, unless you are attempting to clear the callback, but doing that doesn’t make much sense.

## Discussion

This is really not intended for client sessions. Only subclasses would really be interested in using this. They should set these when their subclass object is created, because otherwise they will have no way of receiving the initial command data packet. This is a partner to setEventRefCon, described below.

