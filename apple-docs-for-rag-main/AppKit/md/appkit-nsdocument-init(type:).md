

- AppKit
- NSDocument
-  init(type:) 

Initializer

# init(type:)

Initializes a document of a specified type.

macOS

``` source
@MainActor
convenience init(type typeName: String) throws
```

## Parameters 

`typeName`  

The string that identifies the document type.

## Return Value

The initialized `NSDocument` object, or, if the document could not be created, `nil`.

## Discussion

The default implementation of this method just invokes `[self init]` and `[self setFileType:typeName]`.

You can override this method to perform initialization that must be done when creating new documents but should not be done when opening existing documents. Your override should typically invoke `super`, or at least it must invoke init(), the `NSDocument` designated initializer, to initialize the `NSDocument` private instance variables.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating a Document Object

init()

Initializes and returns an empty document object.

convenience init(contentsOf: URL, ofType: String) throws

Initializes a document located by a URL of a specified type.

convenience init(for: URL?, withContentsOf: URL, ofType: String) throws

Initializes a document with the specified contents, and places the resulting document’s file at the designated location.

