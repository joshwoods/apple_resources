

- Core Data
- NSPersistentStoreCoordinator
-  registeredStoreTypes 

Type Property

# registeredStoreTypes

The coordinator’s registered store types.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class var registeredStoreTypes: [String : NSValue] { get }
```

## Return Value

A dictionary of the registered store types—the keys are the store type strings, and the values are the NSPersistentStore subclasses.

## See Also

### Registering store types

class func registerStoreClass(AnyClass?, type: NSPersistentStore.StoreType)

Registers a persistent store subclass using the specified store type.

class func registerStoreClass(AnyClass?, forStoreType: String)

Registers a persistent store subclass using the specified store type identifier.

Deprecated

