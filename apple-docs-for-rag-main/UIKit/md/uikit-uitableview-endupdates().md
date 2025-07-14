

- UIKit
- UITableView
-  endUpdates() 

Instance Method

# endUpdates()

Concludes a series of method calls that insert, delete, select, or reload rows and sections of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func endUpdates()
```

## Discussion

Use the performBatchUpdates(_:completion:) method instead of this one whenever possible.

You call this method to bracket a series of method calls that begins with beginUpdates() and that consists of operations to insert, delete, select, and reload rows and sections of the table view. When you call `endUpdates`, `UITableView` animates the operations simultaneously. Invocations of beginUpdates() and `endUpdates` can be nested. If you don’t make the insertion, deletion, and selection calls inside this block, table attributes such as row count can become invalid.

## See Also

### Performing batch updates to rows and sections

func performBatchUpdates((() -> Void)?, completion: ((Bool) -> Void)?)

Animates multiple insert, delete, reload, and move operations as a group.

func beginUpdates()

Begins a series of method calls that insert, delete, or select rows and sections of the table view.

