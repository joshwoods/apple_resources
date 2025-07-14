

- UIKit
- UINavigationItem
-  init(title:) 

Initializer

# init(title:)

Creates a navigation item with the specified title.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(title: String)
```

## Parameters 

`title`  

The string to set as the navigation item’s title displayed in the center of the navigation bar.

## Return Value

A new UINavigationItem object initialized with the specified title.

## Discussion

This is the designated initializer for this class.

## See Also

### Related Documentation

var title: String?

The navigation item’s title that displays in the navigation bar.

### Initializing an item

init?(coder: NSCoder)

Creates a navigation item from data in an unarchiver.

