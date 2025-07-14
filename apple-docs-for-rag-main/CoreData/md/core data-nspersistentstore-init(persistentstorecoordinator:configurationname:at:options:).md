

- Core Data
- NSPersistentStore
-  init(persistentStoreCoordinator:configurationName:at:options:) 

Initializer

# init(persistentStoreCoordinator:configurationName:at:options:)

Returns a store initialized with the given arguments.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    persistentStoreCoordinator root: NSPersistentStoreCoordinator?,
    configurationName name: String?,
    at url: URL,
    options: [AnyHashable : Any]? = nil
)
```

## Parameters 

`root`  

A persistent store coordinator.

`name`  

The name of the managed object model configuration to use. Pass `nil` if you do not want to specify a configuration.

`url`  

The URL of the store to load.

`options`  

A dictionary containing configuration options. See NSPersistentStoreCoordinator for a list of key names for options in this dictionary.

## Return Value

A new store object, associated with `coordinator`, that represents a persistent store at url using the options in `options` and—if it is not `nil`—the managed object model configuration `configurationName`.

## Discussion

You must ensure that you load metadata during initialization and set it using metadata.

### Special Considerations

This is the designated initializer for persistent stores.

## See Also

### Related Documentation

var metadata: [String : Any]!

The metadata for the persistent store.

Core Data Programming Guide

Atomic Store Programming Topics

Incremental Store Programming Guide

