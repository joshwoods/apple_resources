

- Foundation
- NSOrderedSet
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

A key-path, relative to the set, for which observer is registered to receive KVO change notifications. This value must not be nil.

`context`  

The context passed to the notifications.

## Discussion

`NSOrderedSet` objects are not observable, so this method raises an exception when invoked on an `NSOrderedSet` object. Instead of observing an ordered set, observe the to-many relationship for which the ordered set is the collection of related objects.

## See Also

### Key-Value Observing Support

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

