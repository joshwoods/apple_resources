

- UIKit
- UIDataSourceModelAssociation
-  modelIdentifierForElement(at:in:) 

Instance Method

# modelIdentifierForElement(at:in:)

Returns the string that uniquely identifies the data at the specified location in the view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func modelIdentifierForElement(
    at idx: IndexPath,
    in view: UIView
) -> String?
```

**Required**

## Parameters 

`idx`  

The index path to the requested data object.

`view`  

The view that contains the data object.

## Return Value

A string that uniquely identifies the data object.

## Discussion

Use the provided information to locate the requested data object. From that object, extract a string that can be used later to identify the same piece of data again. The string you return must not be based on transient information, such as the pointer to the current object in memory; it must instead be tied to the underlying data. In fact, if two different in-memory objects represent the same piece of data in your app, they must both return the same model identifier string.

## See Also

### Locating the data

func indexPathForElement(withModelIdentifier: String, in: UIView) -> IndexPath?

Returns the current index of the data object with the specified identifier.

**Required**

