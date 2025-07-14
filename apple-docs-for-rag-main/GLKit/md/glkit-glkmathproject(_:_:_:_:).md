

- GLKit
-  GLKMathProject(\_:\_:\_:\_:) 

Function

# GLKMathProject(\_:\_:\_:\_:)

Projects a point in object space into the window coordinate system.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMathProject(
    _ object: GLKVector3,
    _ model: GLKMatrix4,
    _ projection: GLKMatrix4,
    _ viewport: UnsafeMutablePointer
) -> GLKVector3
```

## Parameters 

`object`  

The point in object space.

`model`  

A modelview transformation matrix.

`projection`  

A projection matrix.

`viewport`  

A pointer to an array of four integer values. The first pair of values represent the window coordinates of the viewport’s bottom left corner. The second pair of values represent the width and height of the view port.

## Return Value

The projected point in window coordinates.

## See Also

### Projecting Vectors

func GLKMathUnproject(GLKVector3, GLKMatrix4, GLKMatrix4, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Bool>?) -> GLKVector3

Projects a point in view space into object space.

