

- Foundation
- NSArray
-  addObserver(\_:forKeyPath:options:context:) 

Instance Method

# addObserver(\_:forKeyPath:options:context:)

Raises an exception.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addObserver(
    _ observer: NSObject,
    forKeyPath keyPath: String,
    options: NSKeyValueObservingOptions = [],
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`observer`  

The object to register for KVO notifications. The observer must implement the key-value observing method observeValue(forKeyPath:of:change:context:).

`keyPath`  

The key path, relative to the array, of the property to observe. This value must not be `nil`.

`options`  

A combination of NSKeyValueObservingOptions values that specifies what is included in observation notifications.

`context`  

Arbitrary data that is passed to `observer` in observeValue(forKeyPath:of:change:context:).

## Discussion

`NSArray` objects are not observable, so this method raises an exception when invoked on an `NSArray` object. Instead of observing an array, observe the to-many relationship for which the array is the collection of related objects.

## See Also

### Key-Value Observing

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func addObserver(NSObject, toObjectsAt: IndexSet, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Registers an observer to receive key value observer notifications for the specified key-path relative to the objects at the indexes.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String)

Removes `anObserver` from all key value observer notifications associated with the specified `keyPath` relative to the array’s objects at `indexes`.

