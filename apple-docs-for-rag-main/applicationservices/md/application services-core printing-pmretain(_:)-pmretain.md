

- Application Services
- Core Printing
-  PMRetain(\_:) 

Function

# PMRetain(\_:)

Retains a printing object by incrementing its reference count.

macOS 10.0+

``` source
func PMRetain(_ object: PMObject?) -> OSStatus
```

## Parameters 

`object`  

The printing object you want to retain.

## Return Value

A result code. See Result Codes.

## Discussion

You should retain a printing object when you receive it from elsewhere (that is, you did not create or copy it) and you want it to persist. If you retain a printing object, you are responsible for releasing it. (See `PMRelease`.) You can use the function `PMRetain` to increment a printing object’s reference count so that multiple threads or routines can use the object without the risk of another thread or routine deallocating the object.

## See Also

### Releasing and Retaining Printing Objects

func PMRelease(PMObject?) -> OSStatus

Releases a printing object by decrementing its reference count.

