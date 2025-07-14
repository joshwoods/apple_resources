

- File Provider UI
- FPUIActionExtensionViewController
-  prepare(forAction:itemIdentifiers:) 

Instance Method

# prepare(forAction:itemIdentifiers:)

Performs any necessary setup or configuration for the specified action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
func prepare(
    forAction actionIdentifier: String,
    itemIdentifiers: [NSFileProviderItemIdentifier]
)
```

## Parameters 

`actionIdentifier`  

The identifier for the action performed by the user.

`itemIdentifiers`  

The identifiers of the items affected by the action.

## Mentioned in 

Adding Actions to the Context Menu

## Discussion

Use this method to prepare a user interface for handling the action. At a minimum, you should display feedback about the action.

For more information, see Adding Actions to the Context Menu.

## See Also

### Working with Actions

func prepare(forError: any Error)

Performs any necessary setup or configuration when an authentication error occurs.

var extensionContext: FPUIActionExtensionContext

The extension context provided by the host app.

class FPUIActionExtensionContext

An extension context provided to File Provider UI extensions.

