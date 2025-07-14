

- UIKit
- UISearchController
-  init(coder:) 

Initializer

# init(coder:)

Returns an initialized search controller from data in the specified unarchiver.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## Parameters 

`coder`  

An unarchiver object.

## Return Value

An initialized search controller, or `nil` if the coder doesn’t define a search controller.

## See Also

### Creating a search controller

init(searchResultsController: UIViewController?)

Creates and returns a search controller with the specified view controller for displaying the results.

init(nibName: String?, bundle: Bundle?)

Returns an initialized view controller with the nib file in the specified bundle.

