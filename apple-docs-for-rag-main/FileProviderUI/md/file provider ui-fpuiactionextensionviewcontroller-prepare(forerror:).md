

- File Provider UI
- FPUIActionExtensionViewController
-  prepare(forError:) 

Instance Method

# prepare(forError:)

Performs any necessary setup or configuration when an authentication error occurs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
func prepare(forError error: any Error)
```

## Parameters 

`error`  

An object representing the authentication error. Your File Provider extension can pass additional information in the error’s userInfo property.

## Discussion

While your file provider is enumerating its content, the system calls this method whenever your file provider returns an NSFileProviderErrorDomain error with a NSFileProviderError.Code.notAuthenticated code. Use this method to present an interface to authenticate the user.

## See Also

### Working with Actions

func prepare(forAction: String, itemIdentifiers: [NSFileProviderItemIdentifier])

Performs any necessary setup or configuration for the specified action.

var extensionContext: FPUIActionExtensionContext

The extension context provided by the host app.

class FPUIActionExtensionContext

An extension context provided to File Provider UI extensions.

