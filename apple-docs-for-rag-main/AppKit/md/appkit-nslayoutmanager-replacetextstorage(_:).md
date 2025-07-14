

- AppKit
- NSLayoutManager
-  replaceTextStorage(\_:) 

Instance Method

# replaceTextStorage(\_:)

Replaces the layout manager’s current text storage object with the specified object.

macOS 10.7+

``` source
func replaceTextStorage(_ newTextStorage: NSTextStorage)
```

## Parameters 

`newTextStorage`  

The text storage object to set.

## Discussion

Use this method to update the text storage uniformly for a group of related layout manager objects. Unlike changing the value in the textStorage property, this method replaces the text storage for all NSLayoutManager objects that share the current layout manager’s NSTextStorage object.

## See Also

### Accessing the text storage

var textStorage: NSTextStorage?

The text storage object that contains the content to lay out.

