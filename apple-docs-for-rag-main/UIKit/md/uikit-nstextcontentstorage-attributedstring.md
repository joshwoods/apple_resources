

- UIKit
- NSTextContentStorage
-  attributedString 

Instance Property

# attributedString

An attributed string that contains the contents of the document.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@NSCopying
var attributedString: NSAttributedString? { get set }
```

## Discussion

The default value of this property is an NSTextStorage object. When you need to change the text in your view, fetch this string and make your changes to it. When making changes, place them in a block and pass them to the performEditingTransaction(_:) method. Wrapping changes in an edit transaction gives the rest of the text system an opportunity to respond to those changes. For example, the layout manager uses edit transactions to update the text layout for any content in the visible portion of your view.

If you assign a new value to this property, the object replaces the current string with the one you provide. Don’t set the value of this property to `nil`.

