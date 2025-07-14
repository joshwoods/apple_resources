

- ClassKit
- CLSContext
-  init(type:identifier:title:) 

Initializer

# init(type:identifier:title:)

Initializes a new context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
init(
    type: CLSContextType,
    identifier: String,
    title: String
)
```

## Parameters 

`type`  

The context type, like a book chapter, or a game level. This value tells teachers what kind of app content this context represents.

`identifier`  

A string that you create to uniquely identify the context among its siblings. The value must be unique among child contexts of a given parent, but not among contexts with different parents.

`title`  

A human readable name for the new context. The system presents this title to teachers exactly as you store it, so consider localizing it if you distribute your app in more than one locale.

## See Also

### Creating contexts

class CLSObject

The abstract base class for objects managed by ClassKit.

