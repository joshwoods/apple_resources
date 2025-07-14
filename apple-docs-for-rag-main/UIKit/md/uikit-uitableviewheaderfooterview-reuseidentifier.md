

- UIKit
- UITableViewHeaderFooterView
-  reuseIdentifier 

Instance Property

# reuseIdentifier

A string used to identify a reusable header or footer.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var reuseIdentifier: String? { get }
```

## Discussion

You assign a reuse identifier to a header or footer view at creation time. Once assigned, the table view uses that reuse identifier to gather your views when they’re scrolled offscreen and queue them for later reuse. You can retrieve header or footer views by passing the same reuse identifier to the dequeueReusableHeaderFooterView(withIdentifier:) method of the table view.

## See Also

### Managing view reuse

func prepareForReuse()

Prepares a reusable header or footer view for reuse by the table.

