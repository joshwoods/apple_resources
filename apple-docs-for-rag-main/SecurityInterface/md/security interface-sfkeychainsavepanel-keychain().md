

- Security Interface
- SFKeychainSavePanel
-  keychain() 

Instance Method

# keychain()

Returns the keychain created by the keychain save panel.

macOS 10.3+

``` source
@MainActor
func keychain() -> Unmanaged!
```

## See Also

### Returning Information from the Sheet or Panel

func error() -> (any Error)!

Returns the last error encountered by the keychain save panel.

