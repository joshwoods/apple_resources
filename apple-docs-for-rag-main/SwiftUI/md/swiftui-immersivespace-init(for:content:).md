

- SwiftUI
- ImmersiveSpace
-  init(for:content:) 

Initializer

# init(for:content:)

Creates the immersive space for a specified type of presented data.

visionOS 1.0+

``` source
init(
    for type: Data.Type,
    @ImmersiveSpaceContentBuilder content: @escaping (Binding) -> Content
)
```

Show all declarations

## Parameters 

`type`  

The type of presented data this immersive space accepts.

`content`  

An immersive space content builder that defines the content for each instance of the immersive space. The closure receives a binding to the value that you pass to the openImmersiveSpace action when you call that action to open an immersive space. The system automatically persists and restores the value of this binding during state restoration.

## Discussion

The space uses the specified content builder to form the content. Your app invokes this initializer when it presents a value of the specified `type` using the openImmersiveSpace action.

## See Also

### Creating a data-driven immersive space

init(id:for:content:)

Creates the immersive space associated with an identifier for a specified type of presented data.

