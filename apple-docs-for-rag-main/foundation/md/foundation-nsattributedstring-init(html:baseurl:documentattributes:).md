

- Foundation
- NSAttributedString
-  init(HTML:baseURL:documentAttributes:) 

Initializer

# init(HTML:baseURL:documentAttributes:)

Creates an attributed string from the HTML in the specified data object and base URL.

macOS 10.0+

``` source
init?(
    HTML data: Data,
    baseURL base: URL,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

``` source
init?(
    html data: Data,
    baseURL base: URL,
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`data`  

A data object with text in HTML format. The method uses this data to create the attributed string.

`base`  

An NSURL that represents the base URL for all links within the HTML.

`dict`  

An in-out dictionary containing document-level attributes. On output, this method updates the dictionary to contain any document-specific keys found in the data. Specify `nil` if you don’t want the document attributes.

## Return Value

Returns an initialized object, or `nil` if the data can’t be decoded.

## See Also

### Creating from HTML

init?(HTML: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object.

init?(HTML: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object.

class func loadFromHTML(request: URLRequest, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string by converting the contents of the specified HTML URL request.

class func loadFromHTML(fileURL: URL, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string by converting the content of a local HTML file at the specified URL.

class func loadFromHTML(string: String, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string from the specified HTML string.

class func loadFromHTML(data: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string from the specified HTML data.

typealias CompletionHandler

A completion handler for getting an asynchronous attributed string.

