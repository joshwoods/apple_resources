

- AppKit
- NSCollectionViewItem
-  textField 

Instance Property

# textField

A text field outlet that you can use to display a string.

macOS 10.7+

``` source
@IBOutlet @MainActor
weak var textField: NSTextField? { get set }
```

## Discussion

This is a convenience property for accessing a text field in your item’s view hierarchy. Normally, you configure this property in Interface Builder by connecting it to one of your item’s text fields.

## See Also

### Getting and Setting Image and Text Fields

var imageView: NSImageView?

An image view outlet that you can use to display images.

