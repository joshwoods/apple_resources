

- AppKit
- NSObjectController
-  objectClass 

Instance Property

# objectClass

The object class to use when creating new objects.

macOS

``` source
var objectClass: AnyClass! { get set }
```

## Discussion

`NSObjectController`’s default implementation assumes that instances of `objectClass` are initialized using a standard `init` method that takes no arguments.

## See Also

### Related Documentation

var managedObjectContext: NSManagedObjectContext?

The receiver’s managed object context.

var entityName: String?

The entity name used by the receiver to create new objects.

