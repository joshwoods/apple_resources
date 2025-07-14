

- SwiftUI
- ImmersiveSpace
-  init(content:) 

Initializer

# init(content:)

Creates an immersive space.

visionOS 1.0+

``` source
init(@ImmersiveSpaceContentBuilder content: @escaping () -> Content) where Data == Never
```

Show all declarations

## Parameters 

`content`  

An immersive space content builder that defines the content of the space.

## Discussion

The space uses the specified content builder to form the content.

