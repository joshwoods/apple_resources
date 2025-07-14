

- Core Foundation
-  CFMessagePortIsValid(\_:) 

Function

# CFMessagePortIsValid(\_:)

Returns a Boolean value that indicates whether a CFMessagePort object is valid and able to send or receive messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortIsValid(_ ms: CFMessagePort!) -> Bool
```

## Parameters 

`ms`  

The message port to examine.

## Return Value

`true` if `ms` can be used for communication, otherwise `false`.

## See Also

### Examining a Message Port

func CFMessagePortGetContext(CFMessagePort!, UnsafeMutablePointer&lt;CFMessagePortContext>!)

Returns the context information for a CFMessagePort object.

func CFMessagePortGetInvalidationCallBack(CFMessagePort!) -> CFMessagePortInvalidationCallBack!

Returns the invalidation callback function for a CFMessagePort object.

func CFMessagePortGetName(CFMessagePort!) -> CFString!

Returns the name with which a CFMessagePort object is registered.

func CFMessagePortIsRemote(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object represents a remote port.

