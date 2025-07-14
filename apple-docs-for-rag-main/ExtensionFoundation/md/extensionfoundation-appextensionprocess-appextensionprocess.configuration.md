

- ExtensionFoundation
- AppExtensionProcess
-  AppExtensionProcess.Configuration 

Structure

# AppExtensionProcess.Configuration

An object that holds configuration options for an app extension process.

macOS 13.0+

``` source
struct Configuration
```

## Topics

### Handling Process Interruptions

var onInterruption: () -> Void

A closure the system calles when an extension process exits.

### Initializers

init(appExtensionIdentity: AppExtensionIdentity, onInterruption: () -> Void)

### Instance Properties

var appExtensionIdentity: AppExtensionIdentity

## See Also

### Finding or Launching Extensions

init(configuration: AppExtensionProcess.Configuration) throws

Synchronously finds an existing extension process or launches a new one.

init(configuration: AppExtensionProcess.Configuration) async throws

Asynchronously finds an existing extension process or launches a one.

