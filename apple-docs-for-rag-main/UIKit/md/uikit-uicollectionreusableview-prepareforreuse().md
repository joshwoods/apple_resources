

- UIKit
- UICollectionReusableView
-  prepareForReuse() 

Instance Method

# prepareForReuse()

Performs any clean up necessary to prepare the view for use again.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func prepareForReuse()
```

## Discussion

The default implementation of this method does nothing. Subclasses such as UICollectionViewCell override this method and use it to perform relevant actions. So, if your subclass descends from UICollectionViewCell or another intermediate class, call `super` to ensure that your class gets the parent’s behavior.

When the collection view dequeues your view for use, it calls this method before the corresponding dequeue method returns the view to your code. Override this method in your subclass to reset properties to their default values and make the view ready to use again. Don’t use this method to assign any new data to the view; that’s the responsibility of your data source object.

The collection view doesn’t call this method when you use reconfigureItems(at:) on `UICollectionView`, or reconfigureItems(_:) (Swift) or reconfigureItems(withIdentifiers:) (Objective-C) on `NSDiffableDataSourceSnapshot` to update the contents of an existing cell.

## See Also

### Reusing cells

var reuseIdentifier: String?

A string that identifies the purpose of the view.

