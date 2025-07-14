

- Foundation
- NSValue
-  init(SCNMatrix4:) 

Initializer

# init(SCNMatrix4:)

Creates a value object that contains the specified SceneKit 4 x 4 matrix.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**macOS**

``` source
init(SCNMatrix4 v: SCNMatrix4)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
init(SCNMatrix4 v: SCNMatrix4)
```

**macOS**

``` source
init(scnMatrix4 v: SCNMatrix4)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
init(scnMatrix4 v: SCNMatrix4)
```

## Parameters 

`v`  

The value for the new object.

## Return Value

A new value object that contains the matrix information.

## See Also

### Related Documentation

typealias SCNMatrix4 = CATransform3D

A representation of a 4 x 4 matrix.

### Working with SceneKit Vector and Matrix Values

init(SCNVector3: SCNVector3)

Creates a value object that contains the specified three-element SceneKit vector.

init(SCNVector4: SCNVector4)

Creates a value object that contains the specified four-element SceneKit vector.

var scnVector3Value: SCNVector3

The three-element Scene Kit vector representation of the value.

var scnVector4Value: SCNVector4

The four-element Scene Kit vector representation of the value.

var scnMatrix4Value: SCNMatrix4

The Scene Kit 4 x 4 matrix representation of the value.

