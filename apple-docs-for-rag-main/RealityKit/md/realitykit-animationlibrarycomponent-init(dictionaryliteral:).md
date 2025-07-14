

- RealityKit
- AnimationLibraryComponent
-  init(dictionaryLiteral:) 

Initializer

# init(dictionaryLiteral:)

Creates an animation library from a variadic list of key-value pairs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(dictionaryLiteral elements: (String, AnimationResource)...)
```

## Parameters 

`elements`  

A list of key-value pairs that make up the dictionary. Each key is a unique animation name, and each value is an animation resource.

## Discussion

Use the ExpressibleByDictionaryLiteral initializer by directly assigning the library to a dictionary literal.

```
let animationLibrary: AnimationLibraryComponent = [
    "idle": idleAnimation,
    "walk": walkAnimation
]
```

## See Also

### Creating an animation library component

init()

Creates an empty animation library.

init(animations: [String : AnimationResource])

Creates an animation library from a dictionary that associates an animation’s data with its name.

