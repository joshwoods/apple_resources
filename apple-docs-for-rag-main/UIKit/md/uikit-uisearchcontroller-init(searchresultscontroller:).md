

- UIKit
- UISearchController
-  init(searchResultsController:) 

Initializer

# init(searchResultsController:)

Creates and returns a search controller with the specified view controller for displaying the results.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(searchResultsController: UIViewController?)
```

## Parameters 

`searchResultsController`  

The view controller that displays the search results. Specify `nil` if you want to display the search results in the same view controller that displays your searchable content. For apps running in tvOS, provide a results controller because tvOS doesn’t accept `nil` as a valid argument.

## Return Value

An initialized search controller.

## Discussion

After creating the search controller, always assign an object to the searchResultsUpdater property. The search controller uses that object to update the search results.

## See Also

### Creating a search controller

init?(coder: NSCoder)

Returns an initialized search controller from data in the specified unarchiver.

init(nibName: String?, bundle: Bundle?)

Returns an initialized view controller with the nib file in the specified bundle.

