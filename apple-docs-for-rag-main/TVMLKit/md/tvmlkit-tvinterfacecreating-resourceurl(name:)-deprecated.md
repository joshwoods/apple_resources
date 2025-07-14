

- TVMLKit
- TVInterfaceCreating
-  resourceURL(name:) Deprecated

Instance Method

# resourceURL(name:)

Returns a URL for the given resource.

tvOS 9.0–18.0Deprecated

``` source
optional func resourceURL(name resourceName: String) -> URL?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`resourceName`  

A string that contains the name of the resource.

## Return Value

The URL associated with the resource name. The app must return `nil` if the event is not handled.

## Discussion

The `resourceName` parameter comes from a resource URL specified in certain elements. For example, `badge src="resource://developer-resource">` contains the resource name, `developer-resource`.

## See Also

### Retrieving Resource Information

func resourceImage(name: String) -> UIImage?

Returns the image for the given resource

Deprecated

