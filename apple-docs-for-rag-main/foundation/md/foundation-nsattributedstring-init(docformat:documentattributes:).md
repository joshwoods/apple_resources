

- Foundation
- NSAttributedString
-  init(docFormat:documentAttributes:) 

Initializer

# init(docFormat:documentAttributes:)

Creates an attributed string from Microsoft Word format data in the specified data object.

macOS 10.0+

``` source
init?(
    docFormat data: Data,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`data`  

The data from which to create the string.

`dict`  

An in-out dictionary containing document-level attributes. On output, this method updates the dictionary to contain any document-specific keys found in the data. Specify `nil` if you don’t want the document attributes.

## Return Value

Returns an initialized attributed string object, or `nil` if the method can’t decode the data.

## See Also

### Creating from a data file

init(data: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Creates an attributed string from the contents of the specified data object.

init(URL: URL, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Creates an attributed string from the contents of the specified URL.

