

- AppKit
- NSArrayController
-  insert(\_:) 

Instance Method

# insert(\_:)

Creates a new object and inserts it into the receiver’s content array.

macOS

``` source
@IBAction @MainActor
func insert(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

## Discussion

If an entity name is specified (see entityName), this method creates an instance of the of the class specified by the entity, otherwise this method creates an instance of the class specified by objectClass.

### Special Considerations

Beginning with OS X v10.4 the result of this method is deferred until the next iteration of the runloop so that the error presentation mechanism (see Error Responders and Error Recovery) can provide feedback as a sheet.

## See Also

### Inserting

var canInsert: Bool

Returns a Boolean value that indicates whether an object can be inserted into the receiver’s content collection.

