

- SwiftUI
- ImmersiveSpace
-  init(id:content:) 

Initializer

# init(id:content:)

Creates the immersive space associated with the specified identifier.

visionOS 1.0+

``` source
init(
    id: String,
    @ImmersiveSpaceContentBuilder content: () -> Content
) where Data == Never
```

Show all declarations

## Parameters 

`id`  

A string that uniquely identifies the immersive space. Ensure that identifiers are unique among the immersive spaces in your app.

`content`  

An immersive space content builder that defines the content of the space.

## Discussion

The space uses the specified content builder to form the content.

