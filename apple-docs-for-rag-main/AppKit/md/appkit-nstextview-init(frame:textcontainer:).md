

- AppKit
- NSTextView
-  init(frame:textContainer:) 

Initializer

# init(frame:textContainer:)

Initializes a text view.

macOS

``` source
@MainActor
init(
    frame frameRect: NSRect,
    textContainer container: NSTextContainer?
)
```

## Parameters 

`frameRect`  

The frame rectangle of the text view.

`container`  

The text container of the text view.

## Return Value

An initialized text view.

## Discussion

This method is the designated initializer for `NSTextView` objects.

Unlike init(frame:), which builds up an entire group of text-handling objects, you use this method after you’ve created the other components of the text-handling system — a text storage object, a layout manager, and a text container. Assembling the components in this fashion means that the text storage, not the text view, is the principal owner of the component objects.

The init(frame:) initializer uses NSLayoutManager by default. When you use this initializer in macOS 12 and later, you have the option to use NSTextLayoutManager which gives you access to newer TextKit functionality and performance improvements. To use the new layout manager create instances of NSTextLayoutManager, NSTextContainer, and NSTextContentStorage; these manage the view’s text layout, text regions, and backingstore, respectively. The example below shows the order of creation and initialization of these objects, and how configure them to initialize an NSTextView:

```
// The viewWidth and viewBounds are set up elsewhere 
// in the App's initialization.

// Create and initialize the supporting layout, container, and storage management.
let textLayoutManager = NSTextLayoutManager()  
let containerSize = NSSize(width: viewWidth, height: CGFloat.greatestFiniteMagnitude)  
let textContainer = NSTextContainer(size: containerSize)  
textLayoutManager.textContainer = textContainer  
let textContentStorage = NSTextContentStorage()  
textContentStorage.addTextLayoutManager(textLayoutManager)  

let textView = NSTextView(frame: viewBounds, textContainer: textLayoutManager.textContainer)

```

In macOS 11 and earlier, you follow a similar pattern but using NSLayoutManager and NSTextStorage instead:

```
// The viewBounds and containerSize are set up elsewhere 
// in the App's initialization.

// Create and initialize the supporting layout, container, and storage management.
let textContainer = NSTextContainer(size: containerSize)
let layoutManager = NSLayoutManager()
layoutManager.addTextContainer(textContainer)
let textStorage = NSTextStorage()
textStorage.addLayoutManager(layoutManager)

let textView = NSTextView(frame: viewBounds, textContainer: textContainer)

```

## See Also

### Related Documentation

Text System User Interface Layer Programming Guide

Cocoa Text Architecture Guide

### Creating a text view

init(frame: NSRect)

Initializes a text view.

convenience init(usingTextLayoutManager: Bool)

init?(coder: NSCoder)

Initializes a text view with data in an unarchiver.

