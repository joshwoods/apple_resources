

- File Provider
- NSFileProviderExtension
-  placeholderURL(for:) Deprecated

Type Method

# placeholderURL(for:)

Returns a placeholder URL for a given document URL.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func placeholderURL(for url: URL) -> URL
```

Deprecated

Use the NSFileProviderManager class’s placeholderURL(for:) method instead.

## Parameters 

`url`  

The document URL to be converted.

## Return Value

A placeholder URL for the given document.

## Discussion

This method maps file URLs into their corresponding placeholder URLs. You typically call this method to generate the placeholder URL before calling writePlaceholder(at:withMetadata:).

You must not override this method.

## See Also

### Managing placeholders

class func writePlaceholder(at: URL, withMetadata: [URLResourceKey : Any]) throws

Writes a document placeholder with the provided metadata.

Deprecated

