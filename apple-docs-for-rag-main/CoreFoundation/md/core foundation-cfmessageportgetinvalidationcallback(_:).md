

- Core Foundation
-  CFMessagePortGetInvalidationCallBack(\_:) 

Function

# CFMessagePortGetInvalidationCallBack(\_:)

Returns the invalidation callback function for a CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortGetInvalidationCallBack(_ ms: CFMessagePort!) -> CFMessagePortInvalidationCallBack!
```

## Parameters 

`ms`  

The message port to examine.

## Return Value

The callback function invoked when `ms` is invalidated. `NULL` if no callback has been set with CFMessagePortSetInvalidationCallBack(_:_:).

## See Also

### Examining a Message Port

func CFMessagePortGetContext(CFMessagePort!, UnsafeMutablePointer&lt;CFMessagePortContext>!)

Returns the context information for a CFMessagePort object.

func CFMessagePortGetName(CFMessagePort!) -> CFString!

Returns the name with which a CFMessagePort object is registered.

func CFMessagePortIsRemote(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object represents a remote port.

func CFMessagePortIsValid(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object is valid and able to send or receive messages.

