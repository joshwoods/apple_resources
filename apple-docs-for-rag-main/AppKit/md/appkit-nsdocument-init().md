

- AppKit
- NSDocument
-  init() 

Initializer

# init()

Initializes and returns an empty document object.

macOS

``` source
@MainActor
init()
```

## Return Value

An initialized `NSDocument` object.

## Discussion

This initializer (the designated initializer) is invoked by each of the other `NSDocument` initialization methods.

You can override this method to perform initialization that must be done both when creating new empty documents and when opening existing documents. Your override must invoke `super` to initialize private `NSDocument` instance variables. It must never return `nil`. If an error can occur during object initialization, check for the error in an override of init(type:), init(contentsOf:ofType:), or init(for:withContentsOf:ofType:), because those methods can return `NSError` objects.

## See Also

### Related Documentation

Document-Based App Programming Guide for Mac

### Creating a Document Object

convenience init(contentsOf: URL, ofType: String) throws

Initializes a document located by a URL of a specified type.

convenience init(for: URL?, withContentsOf: URL, ofType: String) throws

Initializes a document with the specified contents, and places the resulting document’s file at the designated location.

convenience init(type: String) throws

Initializes a document of a specified type.

