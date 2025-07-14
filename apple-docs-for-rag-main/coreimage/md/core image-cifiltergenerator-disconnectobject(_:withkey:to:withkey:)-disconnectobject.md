

- Core Image
- CIFilterGenerator
-  disconnectObject(\_:withKey:to:withKey:) 

Instance Method

# disconnectObject(\_:withKey:to:withKey:)

Removes the connection between two objects in the filter chain.

macOS 10.5+

``` source
func disconnectObject(
    _ sourceObject: Any,
    withKey sourceKey: String,
    to targetObject: Any,
    withKey targetKey: String
)
```

## Parameters 

`sourceObject`  

A CIFilter object, a CIImage object, or the path (an NSString or NSURL object) to an image.

`sourceKey`  

The key that specifies the source object. Pass `nil` if the source object is used directly.

`targetObject`  

The object from which you want to disconnect the source object.

`targetKey`  

The key that specifies the target that the source object is currently connected to.

## See Also

### Connecting and Disconnecting Objects

func connect(Any, withKey: String?, to: Any, withKey: String)

Adds an object to the filter chain.

