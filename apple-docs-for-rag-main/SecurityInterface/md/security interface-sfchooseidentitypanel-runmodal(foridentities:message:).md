

- Security Interface
- SFChooseIdentityPanel
-  runModal(forIdentities:message:) 

Instance Method

# runModal(forIdentities:message:)

Displays a list of identities in a modal panel.

macOS 10.3+

``` source
@MainActor
func runModal(
    forIdentities identities: [Any]!,
    message: String!
) -> Int
```

## Parameters 

`identities`  

An array of identity objects (objects of type SecIdentity. Use the SecIdentitySearchCopyNext function (in Security/SecIdentitySearch.h) to find identity objects.

`message`  

A message string to display in the panel.

## Discussion

This method returns NSOKButton if the default button is clicked, or NSCancelButton if the alternate button is clicked.

Use the identity() method to obtain the identity chosen by the user.

## Topics

### Related Documentation

func identity() -> Unmanaged&lt;SecIdentity>!

Returns the identity that the user chose in the panel or sheet.

## See Also

### Displaying a Sheet or Panel

func beginSheet(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!, identities: [Any]!, message: String!)

Displays a list of identities in a modal sheet from which the user can select an identity.

