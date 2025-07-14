

- UIKit
- UITab
-  init(title:image:identifier:viewControllerProvider:) 

Initializer

# init(title:image:identifier:viewControllerProvider:)

Creates a tab object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(
    title: String,
    image: UIImage?,
    identifier: String,
    viewControllerProvider: ((UITab) -> UIViewController)? = nil
)
```

## Parameters 

`title`  

The tab’s title.

`image`  

The tab’s image.

`identifier`  

An identifier string for the tab. Each identifier must be unique across all the tabs managed by a UITabBarController.

`viewControllerProvider`  

The view controller that the system presents when someone selects the tab.

## Mentioned in 

Elevating your iPad app with a tab bar and sidebar

