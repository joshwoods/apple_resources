

- UIKit
- UITabGroup
-  init(title:image:identifier:children:viewControllerProvider:) 

Initializer

# init(title:image:identifier:children:viewControllerProvider:)

Creates a tab group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(
    title: String,
    image: UIImage?,
    identifier: String,
    children: [UITab],
    viewControllerProvider: ((UITab) -> UIViewController)? = nil
)
```

## Parameters 

`title`  

The group’s title.

`image`  

The group’s image.

`identifier`  

An identifier string for the tab.

`children`  

The contained tab items.

`viewControllerProvider`  

The view controller that the system presents when someone selects the group from the tab bar.

