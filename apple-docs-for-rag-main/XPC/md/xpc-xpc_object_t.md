

- XPC
-  xpc_object_t 

Type Alias

# xpc_object_t

A type that can describe all XPC objects, including dictionaries, arrays, strings, and numbers.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_object_t = any OS_xpc_object
```

## Discussion

XPC objects are created with a retain count of 1, and therefore it is the caller’s responsibility to call xpc_release on them when they are no longer needed.

## See Also

### Objects

typealias xpc_type_t

A type that describes XPC object types.

protocol OS_xpc_object

The interface for an XPC object.

class OS_xpc_listener

