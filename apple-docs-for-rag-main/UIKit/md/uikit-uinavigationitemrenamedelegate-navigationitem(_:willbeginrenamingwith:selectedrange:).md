

- UIKit
- UINavigationItemRenameDelegate
-  navigationItem(\_:willBeginRenamingWith:selectedRange:) 

Instance Method

# navigationItem(\_:willBeginRenamingWith:selectedRange:)

Tells the delegate when the rename process starts.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
func navigationItem(
    _: UINavigationItem,
    willBeginRenamingWith suggestedTitle: String,
    selectedRange: Range
) -> (String, Range)
```

**Required** Default implementation provided.

## Parameters 

`suggestedTitle`  

The initial text to appear in the rename text field.

`selectedRange`  

The selected range of the initial text in the rename text field.

## Return Value

A string that contains the initial text that appears in the rename text field, and a range that determines which part of that text has selection.

## Discussion

UIKit calls this method when the rename process begins. Implement this method to customize the initial text and text selection that appears in the rename text field.

## Default Implementations

### UINavigationItemRenameDelegate Implementations

func navigationItem(UINavigationItem, willBeginRenamingWith: String, selectedRange: Range&lt;String.Index>) -> (String, Range&lt;String.Index>)

## See Also

### Handling the rename process

func navigationItem(UINavigationItem, didEndRenamingWith: String)

Tells the delegate when the rename process ends.

**Required**

