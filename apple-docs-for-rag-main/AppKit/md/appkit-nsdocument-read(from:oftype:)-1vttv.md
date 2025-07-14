

- AppKit
- NSDocument
-  read(from:ofType:) 

Instance Method

# read(from:ofType:)

Sets the contents of this document by reading from a file or file package, of a specified type, located by a URL.

macOS

``` source
nonisolated
func read(
    from url: URL,
    ofType typeName: String
) throws
```

## Parameters 

`url`  

The location from which the document contents are read.

`typeName`  

The string that identifies the document type.

## Discussion

The default implementation of this method just creates an NSFileWrapper and invokes `[self readFromFileWrapper:theFileWrapper ofType:typeName error:outError]`.

For backward binary compatibility with OS X v10.3 and earlier, the default implementation of this method instead invokes `[self readFromFile:[absoluteURL path] ofType:typeName]` if readFromFile:ofType: is overridden and the URL uses the `file:` scheme.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading the Document’s Content

class func canConcurrentlyReadDocuments(ofType: String) -> Bool

Returns a Boolean value that indicates whether the receiver reads multiple documents of the given type concurrently.

func read(from: FileWrapper, ofType: String) throws

Sets the contents of this document by reading from a file wrapper of a specified type.

func read(from: Data, ofType: String) throws

Sets the contents of this document by reading from data of a specified type.

