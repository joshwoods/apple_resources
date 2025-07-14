

- ContactProvider
- ContactProviderError
-  ContactProviderError.extensionInvalidateTimeout 

Case

# ContactProviderError.extensionInvalidateTimeout

The extension invalidate operation timed out.

iOS 18.0+iPadOS 18.0+

``` source
case extensionInvalidateTimeout
```

## Discussion

This can occur if the extension takes too long to return from invalidate().

## See Also

### Invalidation errors

case extensionInvalidated

The app invalidated the extension while it was enumerating content or changes.

