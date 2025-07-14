

- UIKit
- UITableView
-  beginUpdates() 

Instance Method

# beginUpdates()

Begins a series of method calls that insert, delete, or select rows and sections of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func beginUpdates()
```

## Discussion

Use the performBatchUpdates(_:completion:) method instead of this one whenever possible.

Call this method if you want subsequent insertions, deletion, and selection operations (for example, cellForRow(at:) and indexPathsForVisibleRows) to be animated simultaneously. You can also use this method followed by the endUpdates() method to animate the change in the row heights without reloading the cell. This group of methods must conclude with an invocation of endUpdates(). These method pairs can be nested. If you don’t make the insertion, deletion, and selection calls inside this block, table attributes such as row count might become invalid. You shouldn’t call reloadData() within the group; if you call this method within the group, you must perform any animations yourself.

## See Also

### Performing batch updates to rows and sections

func performBatchUpdates((() -> Void)?, completion: ((Bool) -> Void)?)

Animates multiple insert, delete, reload, and move operations as a group.

func endUpdates()

Concludes a series of method calls that insert, delete, select, or reload rows and sections of the table view.

