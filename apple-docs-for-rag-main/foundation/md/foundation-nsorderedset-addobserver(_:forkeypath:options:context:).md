

- Foundation
- NSOrderedSet
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

The object to register for KVO notifications.

`keyPath`  

The key path, relative to the array, of the property to observe. This value must not be nil.

`options`  

A combination of NSKeyValueObservingOptions values that specifies what is included in observation notifications.

`context`  

Arbitrary data that is passed to observer in observeValue(forKeyPath:of:change:context:).

## Discussion

`NSOrderedSet` objects are not observable, so this method raises an exception when invoked on an `NSOrderedSet` object. Instead of observing an ordered set, observe the to-many relationship for which the ordered set is the collection of related objects.

## See Also

### Key-Value Observing Support

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

