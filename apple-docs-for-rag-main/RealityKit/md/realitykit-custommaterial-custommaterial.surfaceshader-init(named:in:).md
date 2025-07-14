

- RealityKit
- CustomMaterial
- CustomMaterial.SurfaceShader
-  init(named:in:) 

Initializer

# init(named:in:)

Creates a surface shader object from a named function in a Metal library.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    named name: String,
    in library: any MTLLibrary
)
```

## Parameters 

`name`  

The name of the surface shader function.

`library`  

The Metal library that contains the function.

## Discussion

To create a surface shader for a custom material, create a Metal file in your Xcode project. Prefix the function with the keyword `[[visible]]`. The function needs to take a single parameter of type `realitykit::surface_parameters`.

Here’s what a minimal surface shader function looks like:

```
#include 
#include 

// Specify the current default namespace as metal so our code
// doesn't have to to prefix Metal Standard Library symbols.
using namespace metal;

[[visible]] void mySurfaceShader(realitykit::surface_parameters params) {
   // Calculate parameters needed for rendering.
}
```

To create a custom material using this shader, get a reference to your app’s Metal library:

```
guard let device = MTLCreateSystemDefaultDevice() else {
    fatalError("Error creating default metal device.")
}
guard let library = maybeDevice.makeDefaultLibrary() else {
    fatalError("Error creating default metal library")
}
```

Once you have a reference to your Metal library, use it to create the surface shader reference:

```
let surfaceShader = CustomMaterial.SurfaceShader(
    named: "mySurfaceShader",
    in: library
)
```

Important

RealityKit loads surface shader functions by name, so name your surface shader uniquely and to exactly match the `named` parameter.

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

