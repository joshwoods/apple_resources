

- Core Image
- CIFilterGenerator
-  connect(\_:withKey:to:withKey:) 

Instance Method

# connect(\_:withKey:to:withKey:)

Adds an object to the filter chain.

macOS 10.5+

``` source
func connect(
    _ sourceObject: Any,
    withKey sourceKey: String?,
    to targetObject: Any,
    withKey targetKey: String
)
```

## Parameters 

`sourceObject`  

A CIFilter object, a CIImage object, or the path (an NSString or NSURL object) to an image.

`sourceKey`  

The key that specifies the source object. For example, if the source is the output image of a filter, pass the `outputImage` key. Pass `nil` if the source object is used directly.

`targetObject`  

The object to which the source object links.

`targetKey`  

The key that specifies the target for the source. For example, if you are connecting the source to the input image of a CIFilter object, you would pass the `inputImage` key.

## See Also

### Connecting and Disconnecting Objects

func disconnectObject(Any, withKey: String, to: Any, withKey: String)

Removes the connection between two objects in the filter chain.

