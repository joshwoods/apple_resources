

- Foundation
- NSMutableAttributedString
-  read(fromFileURL:options:documentAttributes:) Deprecated

Instance Method

# read(fromFileURL:options:documentAttributes:)

Sets the contents of the receiver from the file at the given URL.

iOS 7.0–9.0DeprecatediPadOS 7.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func read(
    fromFileURL url: URL,
    options opts: [AnyHashable : Any] = [:],
    documentAttributes dict: AutoreleasingUnsafeMutablePointer?
) throws
```

Deprecated

Use read(from:options:documentAttributes:) instead.

## Parameters 

`url`  

The location of the file providing text data.

`opts`  

The option keys for importing the document. For a list of possible values, see “Option keys for importing documents” in NSAttributedString.

`dict`  

On return, contains the document attributes. For a list of possible values, see “Document Attributes” in NSAttributedString.

## Discussion

For RTF formatted files, the contents of the file are appended to the previous string instead of replacing the previous string.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Deprecated

func read(from: Data, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Sets the contents of the receiver from the specified data object`.`

Deprecated

func read(from: URL, options: [AnyHashable : Any], documentAttributes: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Sets the contents of receiver from the file at the specified URL.

Deprecated

