

- UIKit
- UIBarButtonItem
-  init(customView:) 

Initializer

# init(customView:)

Creates an item using the specified custom view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(customView: UIView)
```

## Parameters 

`customView`  

A custom view representing the item.

## Return Value

A newly initialized UIBarButtonItem.

## Discussion

The bar button item created by this method doesn’t call the action method of its target in response to user interactions. Instead, the bar button item expects the specified custom view to handle any user interactions and provide an appropriate response.

