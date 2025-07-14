

- AppKit
- NSPasteboardReading
-  init(pasteboardPropertyList:ofType:) 

Initializer

# init(pasteboardPropertyList:ofType:)

Initializes an instance with a property list object and a type string.

macOS

``` source
init?(
    pasteboardPropertyList propertyList: Any,
    ofType type: NSPasteboard.PasteboardType
)
```

``` source
init?(
    pasteboardPropertyList propertyList: Any,
    ofType type: NSPasteboard.PasteboardType
)
```

**Required**

## Parameters 

`propertyList`  

A property list containing data to initialize the receiver.

By default, the property list object is an instance of `NSData`. If you implement readingOptions(forType:pasteboard:) and specify an option other than asData, the `propertyList` may be any other property list object.

`type`  

A UTI supported by the receiver for reading (one of the types returned by readableTypes(for:)).

## Return Value

An object initialized using the data in `propertyList`.

## Discussion

This method is considered optional because, if readableTypes(for:) returns just a single type, and that type uses the asKeyedArchive reading option, then instances are initialized using init(coder:) instead of this method.

## See Also

### Related Documentation

Drag and Drop Programming Topics

Pasteboard Programming Guide

Services Implementation Guide

