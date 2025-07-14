

- Core Data
- NSPersistentStoreCoordinator
-  registerStoreClass(\_:forStoreType:) Deprecated

Type Method

# registerStoreClass(\_:forStoreType:)

Registers a persistent store subclass using the specified store type identifier.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func registerStoreClass(
    _ storeClass: AnyClass?,
    forStoreType storeType: String
)
```

Deprecated

Use registerStoreClass(_:type:) instead.

## Parameters 

`storeClass`  

The `NSPersistentStore` subclass to use for the store of type `storeType`.

`storeType`  

A unique string that identifies a store type.

## Discussion

You must invoke this method before a custom subclass of NSPersistentStore can be loaded into a persistent store coordinator.

You can pass `nil` for `storeClass` to unregister the store type.

## See Also

### Registering store types

class func registerStoreClass(AnyClass?, type: NSPersistentStore.StoreType)

Registers a persistent store subclass using the specified store type.

class var registeredStoreTypes: [String : NSValue]

The coordinator’s registered store types.

