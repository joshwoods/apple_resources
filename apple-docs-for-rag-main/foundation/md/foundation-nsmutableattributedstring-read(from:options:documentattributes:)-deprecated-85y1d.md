

- Foundation
- NSMutableAttributedString
-  read(from:options:documentAttributes:) Deprecated

Instance Method

# read(from:options:documentAttributes:)

Sets the contents of receiver from the file at the specified URL.

macOS 10.0–10.11Deprecated

``` source
func read(
    from url: URL,
    options: [AnyHashable : Any] = [:],
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

Deprecated

Use read(from:options:documentAttributes:) instead.

## Parameters 

`url`  

The URL of the document to open.

`options`  

The option keys for importing the document. For a list of possible values, see “Option keys for importing documents” in NSAttributedString.

`dict`  

On return, contains the document attributes. For a list of possible values, see “Document Attributes” in NSAttributedString.

## Return Value

true if the attributed string is created successfully or false if it was not.

## Discussion

Filter services can be used to convert the contents of the URL into a format recognized by Cocoa.

## See Also

### Deprecated

func read(from: Data, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Sets the contents of the receiver from the specified data object`.`

Deprecated

func read(fromFileURL: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Sets the contents of the receiver from the file at the given URL.

Deprecated

