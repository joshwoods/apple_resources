

- Foundation
- NSMutableAttributedString
-  endEditing() 

Instance Method

# endEditing()

Ends the buffering of changes to the string’s characters and attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func endEditing()
```

## Discussion

Override this method in a subclass to consolidate changes made since a previous call to beginEditing(). When you call this method, the string notifies observers of the changes.

The default implementation of this method does nothing. Subclasses such as NSTextStorage override this method and use it to tell the layout manager to update the text layout.

## See Also

### Related Documentation

func processEditing()

Cleans up changes to the text storage object and notifies its delegate and layout managers of changes.

### Grouping Changes

func beginEditing()

Begins the buffering of changes to the string’s characters and attributes.

