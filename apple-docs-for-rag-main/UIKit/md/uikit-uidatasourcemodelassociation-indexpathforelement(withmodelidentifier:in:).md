

- UIKit
- UIDataSourceModelAssociation
-  indexPathForElement(withModelIdentifier:in:) 

Instance Method

# indexPathForElement(withModelIdentifier:in:)

Returns the current index of the data object with the specified identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func indexPathForElement(
    withModelIdentifier identifier: String,
    in view: UIView
) -> IndexPath?
```

**Required**

## Parameters 

`identifier`  

The identifier for the requested data object. Use this identifier to locate the matching object in your data source object. This is the same string that your app’s modelIdentifierForElement(at:in:) method returned when encoding the data originally.

`view`  

The view into which the object is being inserted.

## Return Value

The current index of the object whose data matches the value in `identifier`, or `nil` if the object was not found.

## Discussion

During state restoration, `view` can call this method to locate objects that aren’t where they were expected to be. This can happen if the number of objects in the table isn’t the same as during the previous launch cycle. The view uses the information to ensure that the rows with the same data are once again selected or scrolled into view, even if those rows are in a different location now.

## See Also

### Locating the data

func modelIdentifierForElement(at: IndexPath, in: UIView) -> String?

Returns the string that uniquely identifies the data at the specified location in the view.

**Required**

