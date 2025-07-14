

- UIKit
- UIDocument
-  init(fileURL:) 

Initializer

# init(fileURL:)

Returns a document object initialized with its file-system location.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(fileURL url: URL)
```

## Parameters 

`url`  

A file URL identifying the location in the application sandbox where document data is to be written. Passing in `nil` or an empty URL results in the throwing of an invalidArgumentException.

## Return Value

A `UIDocument` object or `nil` if the object could not be created.

## Discussion

After you create a document object and no file exists for it yet, you should next call the save(to:for:completionHandler:) to write the document to its file-system location in the application sandbox. If `url` locates an existing document file, call open(completionHandler:) after creating the document object. The second parameter of this method, the save operation constant, should be UIDocument.SaveOperation.forCreating when there is no document file yet. In the completion handler, if you want the document to be automatically synced with other devices you should ensure that its URL is based in a ubiquitous container; see Designing for Documents in iCloud for more information.

## See Also

### Related Documentation

var fileURL: URL

The file URL you use to initialize the document.

