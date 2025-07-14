

- Foundation
- NSAttributedString
-  init(data:options:documentAttributes:) 

Initializer

# init(data:options:documentAttributes:)

Creates an attributed string from the contents of the specified data object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    data: Data,
    options: [NSAttributedString.DocumentReadingOptionKey : Any] = [:],
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
) throws
```

## Parameters 

`data`  

The data from which to create the string.

`options`  

Attributes for interpreting the document contents. Specify the documentType or fileType option to interpret the data as a specific type. When sharing files between different platforms, specify the sourceTextScaling or targetTextScaling options for any required text scaling behaviors. Specify the characterEncoding attribute for plain-text files. Specify the defaultAttributes key to apply document attributes to the returned string. If you specify an empty dictionary, the method identifies the data format from the data itself.

`dict`  

An in-out dictionary containing document-level attributes. On output, this method updates the dictionary to contain any document-specific keys found in the data. Specify `nil` if you don’t want the document attributes.

## Return Value

Returns an initialized attributed string object, or `nil` if the method can’t decode the data.

## Discussion

Don’t call this method from a background thread if the `options` dictionary includes the documentType attribute with a value of html. If you do, the method tries to synchronize with the main thread, fails, and times out. Calling it from the main thread works, but can still time out if the HTML contains references to external resources. The HTML import mechanism is meant for implementing something like markdown (that is, text styles, colors, and so on), not for general HTML import.

Handling Errors in Swift

In Swift, this API is imported as an initializer and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating from a data file

init?(docFormat: Data, documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Creates an attributed string from Microsoft Word format data in the specified data object.

init(URL: URL, options: [NSAttributedString.DocumentReadingOptionKey : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) throws

Creates an attributed string from the contents of the specified URL.

