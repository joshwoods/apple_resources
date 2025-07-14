

- Swift
- Bool
-  init(\_:) 

Initializer

# init(\_:)

Creates a new Boolean value from the given string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(_ description: String)
```

## Parameters 

`description`  

A string representation of the Boolean value.

## Discussion

If the `description` value is any string other than `"true"` or `"false"`, the result is `nil`. This initializer is case sensitive.

## See Also

### Creating a Boolean From Another Value

init(Bool)

Creates an instance equal to the given Boolean value.

