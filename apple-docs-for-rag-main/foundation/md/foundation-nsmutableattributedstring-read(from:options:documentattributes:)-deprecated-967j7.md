

- Foundation
- NSMutableAttributedString
-  read(from:options:documentAttributes:) Deprecated

Instance Method

# read(from:options:documentAttributes:)

Sets the contents of the receiver from the specified data object`.`

macOS 10.0–10.11Deprecated

``` source
func read(
    from data: Data,
    options: [AnyHashable : Any] = [:],
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

Deprecated

Use read(from:options:documentAttributes:) instead.

## Parameters 

`data`  

The data to read.

`options`  

The option keys for importing the document. For a list of possible values, see “Option keys for importing documents” in NSAttributedString.

`dict`  

On return, contains the document attributes. For a list of possible values, see “Document Attributes” in NSAttributedString.

## Return Value

true if the attributed string is created successfully or false if it was not.

## See Also

### Deprecated

func read(from: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Sets the contents of receiver from the file at the specified URL.

Deprecated

func read(fromFileURL: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Sets the contents of the receiver from the file at the given URL.

Deprecated

