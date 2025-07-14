

- Foundation
- NSArray
-  addObserver(\_:toObjectsAt:forKeyPath:options:context:) 

Instance Method

# addObserver(\_:toObjectsAt:forKeyPath:options:context:)

Registers an observer to receive key value observer notifications for the specified key-path relative to the objects at the indexes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addObserver(
    _ observer: NSObject,
    toObjectsAt indexes: IndexSet,
    forKeyPath keyPath: String,
    options: NSKeyValueObservingOptions = [],
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`observer`  

The observer.

`indexes`  

The index set.

`keyPath`  

The key path, relative to the array, to be observed.

`options`  

The options to be included in the notification.

`context`  

The context passed to the notifications.

## Discussion

The `options` determine what is included in the notifications, and the `context` is passed in the notifications.

This is not merely a convenience method; invoking this method is potentially much faster than repeatedly invoking addObserver(_:forKeyPath:options:context:).

## See Also

### Key-Value Observing

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String)

Removes `anObserver` from all key value observer notifications associated with the specified `keyPath` relative to the array’s objects at `indexes`.

