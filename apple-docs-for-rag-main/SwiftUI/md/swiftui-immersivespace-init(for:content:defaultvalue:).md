

- SwiftUI
- ImmersiveSpace
-  init(for:content:defaultValue:) 

Initializer

# init(for:content:defaultValue:)

Creates an immersive space.

visionOS 1.0+

``` source
init(
    for type: Data.Type = Data.self,
    @ImmersiveSpaceContentBuilder content: @escaping (Binding) -> Content,
    defaultValue: @escaping () -> Data
)
```

Show all declarations

## Parameters 

`type`  

The type of presented data this immersive space accepts.

`content`  

An immersive space content builder that defines the content for each instance of the immersive space. The closure receives a binding to the value that you pass to the openImmersiveSpace action when you call that action to open an immersive space. The system automatically persists and restores the value of this binding during state restoration.

`defaultValue`  

A closure that returns a value that SwiftUI presents when it doesn’t receive one from you, like when you call the openImmersiveSpace action without providing a value.

## Discussion

The immersive space uses the specified content builder as a template to form the content of the space. Your app invokes this initializer when it presents a value of the specified `type` using the openImmersiveSpace action.

## See Also

### Providing default data to an immersive space

init(id:for:content:defaultValue:)

Creates the immersive space associated with an identifier for a specified type of presented data, and a default value, if the data is not set.

