

- File Provider UI
- FPUIActionExtensionViewController
-  extensionContext 

Instance Property

# extensionContext

The extension context provided by the host app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
var extensionContext: FPUIActionExtensionContext { get }
```

## See Also

### Working with Actions

func prepare(forAction: String, itemIdentifiers: [NSFileProviderItemIdentifier])

Performs any necessary setup or configuration for the specified action.

func prepare(forError: any Error)

Performs any necessary setup or configuration when an authentication error occurs.

class FPUIActionExtensionContext

An extension context provided to File Provider UI extensions.

