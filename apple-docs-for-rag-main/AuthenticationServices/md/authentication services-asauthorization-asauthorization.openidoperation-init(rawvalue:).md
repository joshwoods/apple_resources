

- Authentication Services
- ASAuthorization
- ASAuthorization.OpenIDOperation
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates an operation from the given string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

The name of the operation.

## Discussion

Typically you use one of the predefined operations, like operationLogin, instead of initializing one from a string.

## See Also

### Creating an Operation

init(String)

Creates an operation from the given string.

