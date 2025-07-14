

- File Provider
- NSFileProviderExtension
-  writePlaceholder(at:withMetadata:) Deprecated

Type Method

# writePlaceholder(at:withMetadata:)

Writes a document placeholder with the provided metadata.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func writePlaceholder(
    at placeholderURL: URL,
    withMetadata metadata: [URLResourceKey : Any]
) throws
```

Deprecated

Use the NSFileProviderManager class’s writePlaceholder(at:withMetadata:) method instead.

## Parameters 

`placeholderURL`  

The placeholder URL for the document. You can generate a placeholder URL from a document URL by calling placeholderURL(for:).

`metadata`  

The metadata for this document.

## Discussion

Call this method whenever you need to create a placeholder for a document. The metadata that you provide depends largely on the needs of your document picker’s user interface; however, the common options include file size, filename, and thumbnails.

You must not override this method.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Managing placeholders

class func placeholderURL(for: URL) -> URL

Returns a placeholder URL for a given document URL.

Deprecated

