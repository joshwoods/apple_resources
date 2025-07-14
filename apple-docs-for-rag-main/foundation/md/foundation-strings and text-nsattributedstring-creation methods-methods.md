

- Foundation
- Strings and Text
- NSAttributedString
-  Creation methods 

API Collection

# Creation methods

Create attributed strings from existing content or raw text and apply the initial attributes.

## Topics

### Creating from another string

init(string: String)

Creates an attributed string with the specified text and no attribute information.

init(string: String, attributes: [NSAttributedString.Key : Any]?)

Creates an attributed string with the specified text and attributes.

init(attributedString: NSAttributedString)

Creates a new attributed string from the contents of another attributed string.

### Creating a formatted string

convenience init(AttributedString)

Creates a reference-type attributed string from the specified value-type attributed string.

convenience init&lt;S>(AttributedString, including: S.Type) throws

Creates a reference-type attributed string from the specified value-type attributed string, including an attribute scope.

convenience init&lt;S>(AttributedString, including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates a reference-type attributed string from the specified value-type attributed string, including an attribute scope that a key path identifies.

### Creating from a data file

init(data: Data, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Creates an attributed string from the contents of the specified data object.

init?(docFormat: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from Microsoft Word format data in the specified data object.

init(URL: URL, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Creates an attributed string from the contents of the specified URL.

### Creating from HTML

init?(HTML: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object.

init?(HTML: Data, baseURL: URL, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the HTML in the specified data object and base URL.

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

### Creating from RTF

init?(RTF: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTF commands and data in the specified data object.

init?(RTFD: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string by decoding the stream of RTFD commands and data in the specified data object.

init?(RTFDFileWrapper: FileWrapper, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from the specified file wrapper that contains an RTFD document.

### Creating from markdown

convenience init(markdown: String, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from a Markdown-formatted string using the provided options.

convenience init(markdown: Data, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from Markdown-formatted data using the provided options.

convenience init(contentsOf: URL, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified URL that contains Markdown-formatted data using the provided options.

### Creating a string with an attachment

init(attachment: NSTextAttachment)

Creates an attributed string with an attachment.

convenience init(attachment: NSTextAttachment, attributes: [NSAttributedString.Key : Any])

Creates an attributed string with an attachment and applies the specified attributes to it.

convenience init(adaptiveImageGlyph: NSAdaptiveImageGlyph, attributes: [NSAttributedString.Key : Any])

Creates an attributed string with an adaptive image glyph and applies the specified attributes to it.

