

- Foundation
- NSAttributedString
-  loadFromHTML(fileURL:options:completionHandler:) 

Type Method

# loadFromHTML(fileURL:options:completionHandler:)

Creates an attributed string by converting the content of a local HTML file at the specified URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func loadFromHTML(
    fileURL: URL,
    options: [NSAttributedString.DocumentReadingOptionKey : Any] = [:],
    completionHandler: @escaping NSAttributedString.CompletionHandler
)
```

``` source
class func fromHTML(
    fileURL: URL,
    options: [NSAttributedString.DocumentReadingOptionKey : Any] = [:]
) async throws -> (NSAttributedString, [NSAttributedString.DocumentAttributeKey : Any])
```

## Parameters 

`fileURL`  

A URL that specifies the file to load.

`options`  

Specifies additional options for loading the document. For a list of possible keys, see NSAttributedStringDocumentReadingOptionKey.

`completionHandler`  

A completion handler to execute with the results.

## See Also

### Creating from HTML

init?(HTML: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object.

init?(HTML: Data, baseURL: URL, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object and base URL.

init?(HTML: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object.

class func loadFromHTML(request: URLRequest, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string by converting the contents of the specified HTML URL request.

class func loadFromHTML(string: String, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string from the specified HTML string.

class func loadFromHTML(data: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], completionHandler: NSAttributedString.CompletionHandler)

Creates an attributed string from the specified HTML data.

typealias CompletionHandler

A completion handler for getting an asynchronous attributed string.

