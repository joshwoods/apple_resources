

- TVMLKit
- TVInterfaceCreating
-  resourceImage(name:) Deprecated

Instance Method

# resourceImage(name:)

Returns the image for the given resource

tvOS 9.0–18.0Deprecated

``` source
optional func resourceImage(name resourceName: String) -> UIImage?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`resourceName`  

A string that contains the name of the resource.

## Return Value

The UIImage associated with the resource name. Returns `nil` if no image matches the resource name or if the event is not handled.

## Discussion

The `resourceName` parameter comes from a resource URL specified in certain elements. For example, ```  ``` contains the resource name, `developer-resource`.

## See Also

### Retrieving Resource Information

func resourceURL(name: String) -> URL?

Returns a URL for the given resource.

Deprecated

