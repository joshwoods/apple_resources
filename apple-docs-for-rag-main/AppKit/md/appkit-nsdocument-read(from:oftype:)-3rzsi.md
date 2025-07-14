

- AppKit
- NSDocument
-  read(from:ofType:) 

Instance Method

# read(from:ofType:)

Sets the contents of this document by reading from a file wrapper of a specified type.

macOS

``` source
nonisolated
func read(
    from fileWrapper: FileWrapper,
    ofType typeName: String
) throws
```

## Parameters 

`fileWrapper`  

The file wrapper from which the document contents are read.

`typeName`  

The string that identifies the document type.

## Discussion

The default implementation of this method invokes `[self readFromData:[fileWrapper regularFileContents] ofType:typeName error:outError]`.

For backward binary compatibility with OS X v10.3 and earlier, the default implementation of this method instead invokes `[self loadFileWrapperRepresentation:fileWrapper ofType:typeName]` if loadFileWrapperRepresentation:ofType: is overridden.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading the Document’s Content

class func canConcurrentlyReadDocuments(ofType: String) -> Bool

Returns a Boolean value that indicates whether the receiver reads multiple documents of the given type concurrently.

func read(from: URL, ofType: String) throws

Sets the contents of this document by reading from a file or file package, of a specified type, located by a URL.

func read(from: Data, ofType: String) throws

Sets the contents of this document by reading from data of a specified type.

