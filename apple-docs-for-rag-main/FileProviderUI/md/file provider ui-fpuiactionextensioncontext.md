

- File Provider UI
-  FPUIActionExtensionContext 

Class

# FPUIActionExtensionContext

An extension context provided to File Provider UI extensions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+

``` source
class FPUIActionExtensionContext
```

## Mentioned in 

Adding Actions to the Context Menu

## Topics

### Completing the Action

func completeRequest()

Marks the action as complete.

func cancelRequest(withError: any Error)

Cancels the action and returns the provided error.

### Identifying the Domain

var domainIdentifier: NSFileProviderDomainIdentifier?

The identifier for the domain managed by the current file provider.

struct NSFileProviderDomainIdentifier

A unique identifier for a file provider’s domain.

## Relationships

### Inherits From

- NSExtensionContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with Actions

func prepare(forAction: String, itemIdentifiers: [NSFileProviderItemIdentifier])

Performs any necessary setup or configuration for the specified action.

func prepare(forError: any Error)

Performs any necessary setup or configuration when an authentication error occurs.

var extensionContext: FPUIActionExtensionContext

The extension context provided by the host app.

