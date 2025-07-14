

- UIKit
- UICollectionReusableView
-  reuseIdentifier 

Instance Property

# reuseIdentifier

A string that identifies the purpose of the view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var reuseIdentifier: String? { get }
```

## Discussion

The collection view identifies and queues reusable views using their reuse identifiers. The collection view sets this value when it first creates the view, and the value cannot be changed later. When your data source is prompted to provide a given view, it can use the reuse identifier to dequeue a view of the appropriate type.

## See Also

### Reusing cells

func prepareForReuse()

Performs any clean up necessary to prepare the view for use again.

