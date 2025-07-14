

- Foundation
- NSAttributedString
-  init(path:documentAttributes:) Deprecated

Initializer

# init(path:documentAttributes:)

Initializes a new attribute string object from RTF or RTFD data in the file at the specified path.

macOS 10.0–10.11Deprecated

``` source
init?(
    path: String,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

Deprecated

Use init(URL:options:documentAttributes:) instead.

## Parameters 

`path`  

The path to an RTF or RTFD file.

`dict`  

An in-out dictionary containing document-level attributes described in `Document Attributes`. May be `NULL`, in which case no document attributes are returned.

## Return Value

Returns an initialized object, or `nil` if the data can’t be decoded.

## Discussion

The contents of `path` will be examined to best load the file in whatever format it’s in. Filter services can be used to convert the file into a format recognized by Cocoa. Also returns by reference in `docAttributes` a dictionary containing document-level attributes described in `Document Attributes`. `docAttributes` may be `NULL`, in which case no document attributes are returned. Returns an initialized object, or `nil` if the file at `path` can’t be decoded.

## See Also

### Deprecated Initializers

init?(URL: URL, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a new attributed string object from the data at the specified URL.

Deprecated

init(fileURL: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Initializes a new attributed string object from the data at the specified URL.

Deprecated

