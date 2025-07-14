

- UIKit
- NSTextContainer
-  replaceLayoutManager(\_:) 

Instance Method

# replaceLayoutManager(\_:)

Replaces the layout manager for the group of text system objects that contains the text container.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func replaceLayoutManager(_ newLayoutManager: NSLayoutManager)
```

## Parameters 

`newLayoutManager`  

The new layout manager.

## Discussion

The framework reassigns all text containers and text views attached to the old layout manager to the new layout manager. Unlike setting the layoutManager property directly, this method makes all the adjustments necessary to keep the text object relationships intact.

## See Also

### Managing text components

var layoutManager: NSLayoutManager?

The text container’s layout manager.

var textLayoutManager: NSTextLayoutManager?

weak var textView: NSTextView? { get set }

The text container’s text view.

