

- Security Interface
- SFKeychainSavePanel
-  setPassword(\_:) 

Instance Method

# setPassword(\_:)

Specifies the password for the keychain that will be created.

macOS 10.3+

``` source
@MainActor
func setPassword(_ password: String!)
```

## Parameters 

`password`  

The password to be used for the new keychain.

## Discussion

This method is optional. If you don’t call this method, the keychain save panel displays a password-entry dialog.

## See Also

### Displaying a Sheet or Panel

func beginSheet(forDirectory: String!, file: String!, modalFor: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays a sheet that allows a user to create a new keychain.

func runModal(forDirectory: String!, file: String!) -> Int

Displays a panel that allows a user to create a new keychain.

