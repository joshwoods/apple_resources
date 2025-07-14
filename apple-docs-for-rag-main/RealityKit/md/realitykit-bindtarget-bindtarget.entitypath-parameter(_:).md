

- RealityKit
- BindTarget
- BindTarget.EntityPath
-  parameter(\_:) 

Instance Method

# parameter(\_:)

Provides a bind target for a particular animated property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
func parameter(_ name: String) -> BindTarget
```

## Parameters 

`name`  

The animated property’s name.

## See Also

### Accessing a bind target

var jointTransforms: BindTarget

A bind target for the entity’s joint transforms.

var transform: BindTarget

A bind target for the entity’s transform.

var `self`: BindTarget

A bind target for the entity.

