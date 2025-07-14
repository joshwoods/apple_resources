

- UIKit
- UINavigationItemRenameDelegate
-  navigationItemShouldBeginRenaming(\_:) 

Instance Method

# navigationItemShouldBeginRenaming(\_:)

Asks the delegate whether the navigation item supports renaming.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
func navigationItemShouldBeginRenaming(_: UINavigationItem) -> Bool
```

**Required** Default implementation provided.

## Return Value

true to support renaming and show Rename in the title menu; otherwise, false.

## Discussion

UIKit calls this method when the navigation bar’s title menu becomes visible to validate whether to show Rename as part of that menu. Implement this method to determine whether to display the Rename menu element and support the rename process.

## Default Implementations

### UINavigationItemRenameDelegate Implementations

func navigationItemShouldBeginRenaming(UINavigationItem) -> Bool

## See Also

### Determining rename support

func navigationItem(UINavigationItem, shouldEndRenamingWith: String) -> Bool

Asks the delegate whether to continue or abandon the rename process.

**Required** Default implementation provided.

