

- Core Foundation
-  CFMessagePortGetName(\_:) 

Function

# CFMessagePortGetName(\_:)

Returns the name with which a CFMessagePort object is registered.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortGetName(_ ms: CFMessagePort!) -> CFString!
```

## Parameters 

`ms`  

The message port to examine.

## Return Value

The registered name of `ms`, `NULL` if unnamed. Ownership follows the The Get Rule.

## See Also

### Examining a Message Port

func CFMessagePortGetContext(CFMessagePort!, UnsafeMutablePointer&lt;CFMessagePortContext>!)

Returns the context information for a CFMessagePort object.

func CFMessagePortGetInvalidationCallBack(CFMessagePort!) -> CFMessagePortInvalidationCallBack!

Returns the invalidation callback function for a CFMessagePort object.

func CFMessagePortIsRemote(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object represents a remote port.

func CFMessagePortIsValid(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object is valid and able to send or receive messages.

