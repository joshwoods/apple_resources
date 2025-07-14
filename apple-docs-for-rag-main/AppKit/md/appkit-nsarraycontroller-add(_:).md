

- AppKit
- NSArrayController
-  add(\_:) 

Instance Method

# add(\_:)

Creates and adds a new object to the receiver’s content and arranged objects.

macOS

``` source
@IBAction @MainActor
func add(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

## Discussion

Beginning with OS X v10.4 the result of this method is deferred until the next iteration of the runloop so that the error presentation mechanism (see Error Responders and Error Recovery) can provide feedback as a sheet.

