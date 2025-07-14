

- RealityKit
- AnimationLibraryComponent
-  init(animations:) 

Initializer

# init(animations:)

Creates an animation library from a dictionary that associates an animation’s data with its name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(animations: [String : AnimationResource])
```

## Parameters 

`animations`  

A dictionary of animation resources that you key by name.

## See Also

### Creating an animation library component

init()

Creates an empty animation library.

init(dictionaryLiteral: (String, AnimationResource)...)

Creates an animation library from a variadic list of key-value pairs.

