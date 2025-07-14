

- UIKit
- UINavigationItemRenameDelegate
-  navigationItem(\_:didEndRenamingWith:) 

Instance Method

# navigationItem(\_:didEndRenamingWith:)

Tells the delegate when the rename process ends.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
func navigationItem(
    _: UINavigationItem,
    didEndRenamingWith title: String
)
```

**Required**

## Parameters 

`title`  

The new title of the navigation item.

## Discussion

UIKit calls this method after a person finishes renaming the navigation item. Implement this method to update your data model with the new title as needed.

UIKit updates the navigation item’s title automatically. However, if you want to modify the final title that the system passes in to this method, you must update the navigation item’s title manually.

## See Also

### Handling the rename process

func navigationItem(UINavigationItem, willBeginRenamingWith: String, selectedRange: Range&lt;String.Index>) -> (String, Range&lt;String.Index>)

Tells the delegate when the rename process starts.

**Required** Default implementation provided.

