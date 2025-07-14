

- RealityKit
- SystemDependency
-  SystemDependency.before(\_:) 

Case

# SystemDependency.before(\_:)

An update order that requests RealityKit update this system before it updates another specified system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case before(any System.Type)
```

## Parameters 

`System`  

A system that this system updates before.

## Mentioned in 

Implementing systems for entities in a scene

## See Also

### Update order

case after(any System.Type)

An update order that requests RealityKit update this system after it updates another specified system.

