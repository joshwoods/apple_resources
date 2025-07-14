

- UIKit
- UITableViewHeaderFooterView
-  prepareForReuse() 

Instance Method

# prepareForReuse()

Prepares a reusable header or footer view for reuse by the table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func prepareForReuse()
```

## Discussion

If your header or footer view is reusable — that is, it has a reuse identifier — the table view calls this method just before returning the view from its dequeueReusableHeaderFooterView(withIdentifier:) method. Subclasses can override this method and use it to reset attributes of the view to their default values. For performance reasons, you should only reset attributes that aren’t related to content.

If the view doesn’t have a reuse identifier, this method is never called.

## See Also

### Managing view reuse

var reuseIdentifier: String?

A string used to identify a reusable header or footer.

