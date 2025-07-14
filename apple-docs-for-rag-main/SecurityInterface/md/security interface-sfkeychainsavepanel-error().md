

- Security Interface
- SFKeychainSavePanel
-  error() 

Instance Method

# error()

Returns the last error encountered by the keychain save panel.

macOS 10.5+

``` source
@MainActor
func error() -> (any Error)!
```

## See Also

### Returning Information from the Sheet or Panel

func keychain() -> Unmanaged&lt;SecKeychain>!

Returns the keychain created by the keychain save panel.

