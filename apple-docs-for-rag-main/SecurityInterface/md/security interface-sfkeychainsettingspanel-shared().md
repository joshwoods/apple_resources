

- Security Interface
- SFKeychainSettingsPanel
-  shared() 

Type Method

# shared()

Returns a shared keychain settings panel object.

macOS 10.3+

``` source
@MainActor
class func shared() -> SFKeychainSettingsPanel!
```

## Discussion

If the shared object has not already been created, this method allocates and initializes the object first.

## See Also

### Related Documentation

Keychain Services Programming Guide

