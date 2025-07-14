

- AppKit
- NSFilePromiseReceiver
-  readableDraggedTypes 

Type Property

# readableDraggedTypes

An array containing dragged file types that are readable.

macOS 10.12+

``` source
class var readableDraggedTypes: [String] { get }
```

## Discussion

A view must register what types it accepts via registerForDraggedTypes(_:). Use that class method to get the file promise drag types that NSFilePromiseReceiver can accept, in order to register a view to accept promised files. NSFilePromiseReceiver can accept file promises from both the item-based NSFilePromiseProvider and the non-item based API. If you don’t register all these drag types, you might not be notified about some file promise drags. Register using the following code:

- Swift
- Objective-C

```
view.registerForDraggedTypes(NSFilePromiseReceiver.readableDraggedTypes())
```

```
[view registerForDraggedTypes:[NSFilePromiseReceiver readableDraggedTypes]];
```

