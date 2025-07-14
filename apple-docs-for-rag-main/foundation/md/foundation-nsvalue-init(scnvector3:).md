

- Foundation
- NSValue
-  init(SCNVector3:) 

Initializer

# init(SCNVector3:)

Creates a value object that contains the specified three-element SceneKit vector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(SCNVector3 v: SCNVector3)
```

``` source
init(scnVector3 v: SCNVector3)
```

## Parameters 

`v`  

The value for the new object.

## Return Value

A new value object that contains the vector information.

## See Also

### Related Documentation

struct SCNVector3

A representation of a three-component vector.

### Working with SceneKit Vector and Matrix Values

init(SCNVector4: SCNVector4)

Creates a value object that contains the specified four-element SceneKit vector.

init(SCNMatrix4: SCNMatrix4)

Creates a value object that contains the specified SceneKit 4 x 4 matrix.

var scnVector3Value: SCNVector3

The three-element Scene Kit vector representation of the value.

var scnVector4Value: SCNVector4

The four-element Scene Kit vector representation of the value.

var scnMatrix4Value: SCNMatrix4

The Scene Kit 4 x 4 matrix representation of the value.

