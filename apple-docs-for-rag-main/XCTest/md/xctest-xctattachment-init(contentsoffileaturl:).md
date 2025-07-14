

- XCTest
- XCTAttachment
-  init(contentsOfFileAtURL:) 

Initializer

# init(contentsOfFileAtURL:)

Creates an attachment from the contents of an existing file on disk.

``` source
convenience init(contentsOfFileAtURL url: URL)
```

``` source
convenience init(contentsOfFile url: URL)
```

## Parameters 

`url`  

The file URL from which data should be read to create the new attachment.

## Discussion

The attachment’s name property is the file name of the provided url. The attachment’s uniformTypeIdentifier value is inferred from the file’s extension. A default UTI of `"public.data"` is used for files without an extension.

Note

Use this initializer with files only. To create an attachment from a directory, use init(compressedContentsOfDirectoryAtURL:).

## See Also

### Creating Attachments from Files and Folders

convenience init(contentsOfFileAtURL: URL, uniformTypeIdentifier: String)

Creates an attachment from the contents of an existing file on disk, with a custom UTI.

Deprecated

convenience init(compressedContentsOfDirectoryAtURL: URL)

Creates an attachment containing a zipped archive of an existing directory on disk.

Deprecated

