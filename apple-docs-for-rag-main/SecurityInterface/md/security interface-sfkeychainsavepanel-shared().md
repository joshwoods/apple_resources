

- Security Interface
- SFKeychainSavePanel
-  shared() 

Type Method

# shared()

Returns a shared keychain save panel object.

macOS 10.3+

``` source
@MainActor
class func shared() -> SFKeychainSavePanel!
```

## Discussion

If the shared object has not already been created, this method allocates and initializes the object first.

## See Also

### Related Documentation

Keychain Services Programming Guide

