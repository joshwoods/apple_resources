

- Security Interface
- SFKeychainSettingsPanel
-  runModal(for:keychain:) 

Instance Method

# runModal(for:keychain:)

Displays a panel that allows users to change keychain settings.

macOS 10.3+

``` source
@MainActor
func runModal(
    for settings: UnsafeMutablePointer!,
    keychain: SecKeychain!
) -> Int
```

## Parameters 

`settings`  

A pointer to a keychain settngs structure. Because this structure is versioned, you must preallocate it and fill in the version of the structure.

`keychain`  

The keychain whose settings you wish to have the user change.

## Discussion

The method result indicates which button the user clicks: NSOKButton or NSCancelButton .

If the user attempts to chanage the settings of a locked keychain, the unlock authorization dialog appears.

## See Also

### Displaying a sheet or panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, settings: UnsafeMutablePointer&lt;SecKeychainSettings>!, keychain: SecKeychain!)

Displays a sheet that allows users to change keychain settings.

