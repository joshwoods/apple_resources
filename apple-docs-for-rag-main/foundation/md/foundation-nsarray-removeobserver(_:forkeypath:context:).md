

- Foundation
- NSArray
-  removeObserver(\_:forKeyPath:context:) 

Instance Method

# removeObserver(\_:forKeyPath:context:)

Raises an exception.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObserver(
    _ observer: NSObject,
    forKeyPath keyPath: String,
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`observer`  

The object to remove as an observer.

`keyPath`  

A key-path, relative to the set, for which `observer` is registered to receive KVO change notifications. This value must not be `nil`.

`context`  

The context passed to the notifications.

## Discussion

`NSArray` objects are not observable, so this method raises an exception when invoked on an `NSArray` object. Instead of observing a array, observe the ordered to-many relationship for which the array is the collection of related objects.

## See Also

### Key-Value Observing

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func addObserver(NSObject, toObjectsAt: IndexSet, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Registers an observer to receive key value observer notifications for the specified key-path relative to the objects at the indexes.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String)

Removes `anObserver` from all key value observer notifications associated with the specified `keyPath` relative to the array’s objects at `indexes`.

