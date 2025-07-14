

- ContactProvider
- ContactProviderError
-  ContactProviderError.extensionInvalidated 

Case

# ContactProviderError.extensionInvalidated

The app invalidated the extension while it was enumerating content or changes.

iOS 18.0+iPadOS 18.0+

``` source
case extensionInvalidated
```

## Discussion

A loaded and enumerating extension can become invalidated for many reasons, including:

- The app invalidates the extension by calling invalidate().

- The app disables the domain by calling disable().

- The app resets the domain by calling reset().

- The person using the app disables the domain in the Settings app.

## See Also

### Invalidation errors

case extensionInvalidateTimeout

The extension invalidate operation timed out.

