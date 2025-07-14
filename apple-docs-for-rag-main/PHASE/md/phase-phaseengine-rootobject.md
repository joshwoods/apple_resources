

- PHASE
- PHASEEngine
-  rootObject 

Instance Property

# rootObject

The main object to which the app adds child objects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var rootObject: PHASEObject { get }
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Discussion

The framework creates and sets the root object at engine instantiation.

Avoid executing the following actions in your app; these actions cause the engine to generate a runtime error:

- Adding this object as a child.

- Altering the transform of this object.

- Copying this object.

