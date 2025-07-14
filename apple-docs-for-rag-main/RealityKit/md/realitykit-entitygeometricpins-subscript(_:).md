

- RealityKit
- EntityGeometricPins
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Obtains a geometric pin the entity owns by name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
subscript(name: String) -> GeometricPin? { get }
```

## Parameters 

`name`  

The name of an existing pin the entity owns.

## Return Value

The pin that associates with the name, or `nil` if no pin with a matching name is found.

