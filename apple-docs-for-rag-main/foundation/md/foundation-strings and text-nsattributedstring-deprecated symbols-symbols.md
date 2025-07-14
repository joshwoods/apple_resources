

- Foundation
- Strings and Text
- NSAttributedString
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Migrate your code away from using these symbols.

## Topics

### Deprecated Initializers

init?(path: String, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a new attribute string object from RTF or RTFD data in the file at the specified path.

Deprecated

init?(URL: URL, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a new attributed string object from the data at the specified URL.

Deprecated

init(fileURL: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Initializes a new attributed string object from the data at the specified URL.

Deprecated

### Deprecated Properties

var containsAttachments: Bool

A Boolean value that indicates whether the attribute string contains any attachment attributes.

Deprecated

### Deprecated Enumerations

enum NSTextWritingDirection

Options for specifying text-writing direction.

Deprecated

### Deprecated Instance Methods

func url(at: Int, effectiveRange: NSRangePointer) -> URL?

Returns a URL, either from a link attribute or from text at the specified location that appears to be a URL string, for use in automatic link detection.

Deprecated

func draw(with: NSRect, options: NSString.DrawingOptions)

Draws the attributed string with the specified options within the specified rectangle in the current graphics context.

Deprecated

func boundingRect(with: NSSize, options: NSString.DrawingOptions) -> NSRect

Calculates and returns a bounding rectangle for the attributed string using the options specified within the specified rectangle in the current graphics context.

Deprecated

