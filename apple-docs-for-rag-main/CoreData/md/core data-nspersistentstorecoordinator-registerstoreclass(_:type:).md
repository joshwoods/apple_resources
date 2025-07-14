

- Core Data
- NSPersistentStoreCoordinator
-  registerStoreClass(\_:type:) 

Type Method

# registerStoreClass(\_:type:)

Registers a persistent store subclass using the specified store type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
class func registerStoreClass(
    _ storeClass: AnyClass?,
    type: NSPersistentStore.StoreType
)
```

## Parameters 

`storeClass`  

A subclass of NSPersistentStore.

`type`  

The store type. For possible values, see NSPersistentStore.StoreType.

## Discussion

You must register the subclass before you load instances of it into the persistent store coordinator. To unregister a subclass for a specific store type, use `nil` for `storeClass`.

## See Also

### Registering store types

class func registerStoreClass(AnyClass?, forStoreType: String)

Registers a persistent store subclass using the specified store type identifier.

Deprecated

class var registeredStoreTypes: [String : NSValue]

The coordinator’s registered store types.

