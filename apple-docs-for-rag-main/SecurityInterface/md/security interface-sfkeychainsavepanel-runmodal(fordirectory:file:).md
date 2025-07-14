

- Security Interface
- SFKeychainSavePanel
-  runModal(forDirectory:file:) 

Instance Method

# runModal(forDirectory:file:)

Displays a panel that allows a user to create a new keychain.

macOS 10.3+

``` source
@MainActor
func runModal(
    forDirectory path: String!,
    file name: String!
) -> Int
```

## Parameters 

`path`  

The path to the folder where the keychain is created. Specify `nil` for `~/Library/Keychains`.

`name`  

The keychain name to be automatically displayed in the Save As field of the panel.

## Discussion

This method returns a result code from the doc://com.apple.documentation/documentation/appkit/nssavepanel/1539053-runmodalfordirectory method of the NSSavePanel class: NSFileHandlingPanelOKButton if the user clicks the OK button or NSFileHandlingPanelCancelButton if the user clicks the Cancel button.

Use the keychain() method to obtain the keychain created by the user.

## See Also

### Displaying a Sheet or Panel

func setPassword(String!)

Specifies the password for the keychain that will be created.

func beginSheet(forDirectory: String!, file: String!, modalFor: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays a sheet that allows a user to create a new keychain.

