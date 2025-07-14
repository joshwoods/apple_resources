

- UIKit
- UISearchContainerViewController
-  init(searchController:) 

Initializer

# init(searchController:)

Initializes and returns a search container view controller with the specified search controller object.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(searchController: UISearchController)
```

## Parameters 

`searchController`  

The search controller managing the search results. This parameter must not be `nil`.

## Return Value

An initialized search container view controller.

## Discussion

After initializing the search container view controller, embed it in your container view controller normally.

