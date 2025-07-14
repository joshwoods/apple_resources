

- AppKit
- NSDocument
-  read(from:ofType:) 

Instance Method

# read(from:ofType:)

Sets the contents of this document by reading from data of a specified type.

macOS

``` source
nonisolated
func read(
    from data: Data,
    ofType typeName: String
) throws
```

## Parameters 

`data`  

The data object from which the document contents are read.

`typeName`  

The string that identifies the document type.

## Discussion

The default implementation of this method throws an exception because at least one of the three reading methods (this method, read(from:ofType:), read(from:ofType:)), or every method that may invoke read(from:ofType:), must be overridden.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading the Document’s Content

class func canConcurrentlyReadDocuments(ofType: String) -> Bool

Returns a Boolean value that indicates whether the receiver reads multiple documents of the given type concurrently.

func read(from: URL, ofType: String) throws

Sets the contents of this document by reading from a file or file package, of a specified type, located by a URL.

func read(from: FileWrapper, ofType: String) throws

Sets the contents of this document by reading from a file wrapper of a specified type.

