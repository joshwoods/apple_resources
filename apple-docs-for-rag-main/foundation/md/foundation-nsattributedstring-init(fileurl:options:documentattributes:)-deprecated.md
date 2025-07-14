

- Foundation
- NSAttributedString
-  init(fileURL:options:documentAttributes:) Deprecated

Initializer

# init(fileURL:options:documentAttributes:)

Initializes a new attributed string object from the data at the specified URL.

iOS 7.0–9.0DeprecatediPadOS 7.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init(
    fileURL url: URL,
    options: [AnyHashable : Any] = [:],
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
) throws
```

Deprecated

Use init(URL:options:documentAttributes:) instead.

## Parameters 

`url`  

An `NSURL` object specifying the document to load.

`options`  

Document attributes for interpreting the document contents. documentType, characterEncoding, and defaultAttributes are supported option keys. If not specified, the method examines the data to attempt to determine the appropriate attributes.

`dict`  

If non-`NULL`, returns a dictionary with various document-wide attributes accessible via document attribute keys.

## Return Value

Returns an initialized attributed string object, or `nil` if the data can’t be decoded.

## Discussion

The HTML importer should not be called from a background thread (that is, the `options` dictionary includes documentType with a value of html). It will try to synchronize with the main thread, fail, and time out. Calling it from the main thread works (but can still time out if the HTML contains references to external resources, which should be avoided at all costs). The HTML import mechanism is meant for implementing something like markdown (that is, text styles, colors, and so on), not for general HTML import.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Deprecated Initializers

init?(path: String, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a new attribute string object from RTF or RTFD data in the file at the specified path.

Deprecated

init?(URL: URL, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a new attributed string object from the data at the specified URL.

Deprecated

