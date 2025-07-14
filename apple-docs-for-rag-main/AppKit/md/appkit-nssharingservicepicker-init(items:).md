

- AppKit
- NSSharingServicePicker
-  init(items:) 

Initializer

# init(items:)

Creates a new sharing service picker for the selected items.

macOS 10.8+

``` source
init(items: [Any])
```

## Parameters 

`items`  

The items to be shared. The items in the array must conform to the NSPasteboardWriting or NSPreviewRepresentableActivityItem protocol. For example, you can specify an NSString, NSImage, NSURL, or similar type directly. You can also specify NSItemProvider or NSDocument objects in the array to share those types.

## Return Value

A configured sharing service picker.

## Discussion

If an item is an NSURL object and contains a file URL (pointing to a video on the local disk for example), the picker shares the content of the file. If the URL is remote, then the picker shares the URL instead of the contents.

