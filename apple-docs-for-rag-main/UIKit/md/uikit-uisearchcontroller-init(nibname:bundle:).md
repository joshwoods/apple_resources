

- UIKit
- UISearchController
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Returns an initialized view controller with the nib file in the specified bundle.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    nibName nibNameOrNil: String?,
    bundle nibBundleOrNil: Bundle?
)
```

## Parameters 

`nibNameOrNil`  

The name of the nib file to associate with the view controller. The nib file name shouldn’t contain any leading path information. If you specify `nil`, the `nibName` property is set to `nil`.

`nibBundleOrNil`  

The bundle in which to search for the nib file. This method looks for the nib file in the bundle’s language-specific project directories first, followed by the Resources directory.

## See Also

### Creating a search controller

init(searchResultsController: UIViewController?)

Creates and returns a search controller with the specified view controller for displaying the results.

init?(coder: NSCoder)

Returns an initialized search controller from data in the specified unarchiver.

