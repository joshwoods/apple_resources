

- UIKit
- UITableView
-  dequeueReusableHeaderFooterView(withIdentifier:) 

Instance Method

# dequeueReusableHeaderFooterView(withIdentifier:)

Returns a reusable header or footer view after locating it by its identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dequeueReusableHeaderFooterView(withIdentifier identifier: String) -> UITableViewHeaderFooterView?
```

## Parameters 

`identifier`  

A string identifying the header or footer view to be reused. This parameter must not be `nil`.

## Return Value

A UITableViewHeaderFooterView object with the associated identifier or `nil` if no such object exists in the reusable view queue.

## Mentioned in 

Adding headers and footers to table sections

## Discussion

For performance reasons, a table view’s delegate should generally reuse UITableViewHeaderFooterView objects when it’s asked to provide them. A table view maintains a queue or list of UITableViewHeaderFooterView objects that the table view’s delegate has marked for reuse. It marks a view for reuse by assigning it a reuse identifier when it creates it (in the init(reuseIdentifier:) method of UITableViewHeaderFooterView).

You can use this method to access specific template header and footer views that you previously created. You can access a view’s reuse identifier through its reuseIdentifier property.

## See Also

### Recycling section headers and footers

func register(UINib?, forHeaderFooterViewReuseIdentifier: String)

Registers a nib object that contains a header or footer with the table view under a specified identifier.

func register(AnyClass?, forHeaderFooterViewReuseIdentifier: String)

Registers a class to use in creating new table header or footer views.

