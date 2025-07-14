

- AppKit
- NSCollectionViewItem
-  imageView 

Instance Property

# imageView

An image view outlet that you can use to display images.

macOS 10.7+

``` source
@IBOutlet @MainActor
weak var imageView: NSImageView? { get set }
```

## Discussion

This is a convenience property for accessing an image view in your item’s view hierarchy. Normally, you configure this property in Interface Builder by connecting it to one of your item’s image views.

## See Also

### Getting and Setting Image and Text Fields

var textField: NSTextField?

A text field outlet that you can use to display a string.

