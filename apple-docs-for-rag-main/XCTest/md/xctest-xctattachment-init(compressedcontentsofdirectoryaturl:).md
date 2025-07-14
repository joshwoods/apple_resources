

- XCTest
- XCTAttachment
-  init(compressedContentsOfDirectoryAtURL:) 

Initializer

# init(compressedContentsOfDirectoryAtURL:)

Creates an attachment containing a zipped archive of an existing directory on disk.

``` source
convenience init(compressedContentsOfDirectoryAtURL url: URL)
```

``` source
convenience init(compressedContentsOfDirectory url: URL)
```

## Parameters 

`url`  

A file URL for a directory whose contents should be compressed.

## Discussion

Zips the contents of the provided directory and wraps the compressed output in an attachment with a uniformTypeIdentifier of `"public.zip-archive"`. The attachment’s name property is set to the name of the zipped directory followed by an extension of `".zip"`.

Available on macOS only.

## See Also

### Creating Attachments from Files and Folders

convenience init(contentsOfFileAtURL: URL)

Creates an attachment from the contents of an existing file on disk.

Deprecated

convenience init(contentsOfFileAtURL: URL, uniformTypeIdentifier: String)

Creates an attachment from the contents of an existing file on disk, with a custom UTI.

Deprecated

