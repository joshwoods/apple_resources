

- UIKit
- UINavigationItemRenameDelegate
-  navigationItem(\_:shouldEndRenamingWith:) 

Instance Method

# navigationItem(\_:shouldEndRenamingWith:)

Asks the delegate whether to continue or abandon the rename process.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
func navigationItem(
    _: UINavigationItem,
    shouldEndRenamingWith title: String
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`title`  

The new title of the navigation item.

## Return Value

true to continue the rename process; false to cancel the rename process.

## Discussion

Implement this method to return false to prevent renaming.

Important

UIKit might not call this method in certain situations, like when the system pushes a new navigation item onto the navigation bar. In these situations, UIKit calls navigationItem(_:didEndRenamingWith:) instead. Therefore, make sure to implement navigationItem(_:didEndRenamingWith:) to handle the cases when navigationItem(_:shouldEndRenamingWith:) returns false.

## Default Implementations

### UINavigationItemRenameDelegate Implementations

func navigationItem(UINavigationItem, shouldEndRenamingWith: String) -> Bool

## See Also

### Determining rename support

func navigationItemShouldBeginRenaming(UINavigationItem) -> Bool

Asks the delegate whether the navigation item supports renaming.

**Required** Default implementation provided.

