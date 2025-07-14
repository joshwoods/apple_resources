

- Core Foundation
-  CFMessagePortIsRemote(\_:) 

Function

# CFMessagePortIsRemote(\_:)

Returns a Boolean value that indicates whether a CFMessagePort object represents a remote port.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortIsRemote(_ ms: CFMessagePort!) -> Bool
```

## Parameters 

`ms`  

The message port to examine.

## Return Value

`true` if `ms` is a remote port, otherwise `false`.

## See Also

### Examining a Message Port

func CFMessagePortGetContext(CFMessagePort!, UnsafeMutablePointer&lt;CFMessagePortContext>!)

Returns the context information for a CFMessagePort object.

func CFMessagePortGetInvalidationCallBack(CFMessagePort!) -> CFMessagePortInvalidationCallBack!

Returns the invalidation callback function for a CFMessagePort object.

func CFMessagePortGetName(CFMessagePort!) -> CFString!

Returns the name with which a CFMessagePort object is registered.

func CFMessagePortIsValid(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object is valid and able to send or receive messages.

