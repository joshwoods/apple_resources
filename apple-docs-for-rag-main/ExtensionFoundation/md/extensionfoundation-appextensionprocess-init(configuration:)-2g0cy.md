

- ExtensionFoundation
- AppExtensionProcess
-  init(configuration:) 

Initializer

# init(configuration:)

Synchronously finds an existing extension process or launches a new one.

macOS 13.0+

``` source
init(configuration: AppExtensionProcess.Configuration) throws
```

## Parameters 

`configuration`  

The configuration options for the process to find or launch.

## Discussion

This initializer finds an existing extension process that matches the provided configuration object. If it’s unable to find an existing process, it launches a new extension process.

## See Also

### Finding or Launching Extensions

init(configuration: AppExtensionProcess.Configuration) async throws

Asynchronously finds an existing extension process or launches a one.

struct Configuration

An object that holds configuration options for an app extension process.

