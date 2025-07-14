

- Core Foundation
-  CFMessagePortGetContext(\_:\_:) 

Function

# CFMessagePortGetContext(\_:\_:)

Returns the context information for a CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortGetContext(
    _ ms: CFMessagePort!,
    _ context: UnsafeMutablePointer!
)
```

## Parameters 

`ms`  

The message port to examine.

`context`  

A pointer to the structure into which the context information for `ms` is to be copied. The information being returned is usually the same information you passed to CFMessagePortCreateLocal(_:_:_:_:_:) when creating `ms`. However, if CFMessagePortCreateLocal(_:_:_:_:_:) returned a cached object instead of creating a new object, `context` is filled with information from the original message port instead of the information you passed to the function.

## Discussion

The context version number for message ports is currently `0`. Before calling this function, you need to initialize the `version` member of `context` to `0`.

## See Also

### Examining a Message Port

func CFMessagePortGetInvalidationCallBack(CFMessagePort!) -> CFMessagePortInvalidationCallBack!

Returns the invalidation callback function for a CFMessagePort object.

func CFMessagePortGetName(CFMessagePort!) -> CFString!

Returns the name with which a CFMessagePort object is registered.

func CFMessagePortIsRemote(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object represents a remote port.

func CFMessagePortIsValid(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object is valid and able to send or receive messages.

