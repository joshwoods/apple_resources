

- InputMethodKit
- IMKServer
-  init(name:controllerClass:delegateClass:) 

Initializer

# init(name:controllerClass:delegateClass:)

Creates and returns a server object initialized with the provided parameters.

macOS 10.5+

``` source
init!(
    name: String!,
    controllerClass controllerClassID: AnyClass!,
    delegateClass delegateClassID: AnyClass!
)
```

## Parameters 

`name`  

The name to initialize the server object with.

`controllerClassID`  

The id for the input controller class.

`delegateClassID`  

The id for the delegate class.

## Return Value

An initialized server object.

## See Also

### Initializing a Server Object

init!(name: String!, bundleIdentifier: String!)

Creates and returns a server object from property list information contained in the provided bundle.

