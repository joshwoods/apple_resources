

- XCTest
- XCTAttachment
-  init(contentsOfFileAtURL:uniformTypeIdentifier:) 

Initializer

# init(contentsOfFileAtURL:uniformTypeIdentifier:)

Creates an attachment from the contents of an existing file on disk, with a custom UTI.

``` source
convenience init(
    contentsOfFileAtURL url: URL,
    uniformTypeIdentifier identifier: String
)
```

``` source
convenience init(
    contentsOfFile url: URL,
    uniformTypeIdentifier identifier: String
)
```

## Parameters 

`url`  

The file URL from which data should be read to create the new attachment.

`identifier`  

A custom UTI to represent the file’s content type.

## Discussion

The attachment’s name property is the file name of the provided url.

Note

Use this initializer with files only. To create an attachment from a directory, use init(compressedContentsOfDirectoryAtURL:).

## See Also

### Creating Attachments from Files and Folders

convenience init(contentsOfFileAtURL: URL)

Creates an attachment from the contents of an existing file on disk.

Deprecated

convenience init(compressedContentsOfDirectoryAtURL: URL)

Creates an attachment containing a zipped archive of an existing directory on disk.

Deprecated

