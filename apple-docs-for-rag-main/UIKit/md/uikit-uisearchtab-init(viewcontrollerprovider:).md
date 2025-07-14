

- UIKit
- UISearchTab
-  init(viewControllerProvider:) 

Initializer

# init(viewControllerProvider:)

Creates a search tab with a system localized title and image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(viewControllerProvider: ((UITab) -> UIViewController)? = nil)
```

## Parameters 

`viewControllerProvider`  

The view controller that the system presents when someone selects the tab.

