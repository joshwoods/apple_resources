

- UIKit
- UIActivityItemProvider
-  init(placeholderItem:) 

Initializer

# init(placeholderItem:)

Initializes and returns a provider object with the specified placeholder data.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(placeholderItem: Any)
```

## Parameters 

`placeholderItem`  

An object that can stand in for the actual object you plan to create. The contents of the object may be empty but the class of the object must match the class of the object you plan to provide later.

## Return Value

An initialized provider object.

