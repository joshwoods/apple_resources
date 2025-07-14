

- Foundation
- NSAttributedString
-  init(URL:documentAttributes:) Deprecated

Initializer

# init(URL:documentAttributes:)

Initializes a new attributed string object from the data at the specified URL.

macOS 10.0–10.11Deprecated

``` source
init?(
    URL url: URL,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

``` source
init?(
    url: URL,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

Deprecated

Use init(URL:options:documentAttributes:) instead.

## Parameters 

`url`  

An `NSURL` object specifying the document to load.

`dict`  

An in-out dictionary containing document-level attributes described in `Document Attributes`. May be `NULL`, in which case no document attributes are returned.

## Return Value

Returns an initialized object, or `nil` if the data can’t be decoded.

## Discussion

The contents of `aURL` are examined to best load the file in whatever format it’s in. Filter services can be used to convert the file into a format recognized by Cocoa. Also returns by reference in `docAttributes` a dictionary containing document-level attributes described in `Document Attributes`. `docAttributes` may be `NULL`, in which case no document attributes are returned. Returns an initialized object, or `nil` if the file at `path` can’t be decoded.

## See Also

### Deprecated Initializers

init?(path: String, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a new attribute string object from RTF or RTFD data in the file at the specified path.

Deprecated

init(fileURL: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Initializes a new attributed string object from the data at the specified URL.

Deprecated

