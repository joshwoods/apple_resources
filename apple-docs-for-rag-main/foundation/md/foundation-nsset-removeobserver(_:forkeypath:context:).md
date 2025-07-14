

- Foundation
- NSSet
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

Arbitrary data that is passed to `observer` in observeValue(forKeyPath:of:change:context:).

## Discussion

`NSSet` objects are not observable, so this method raises an exception when invoked on an `NSSet` object. Instead of observing a set, observe the unordered to-many relationship for which the set is the collection of related objects.

## See Also

### Key-Value Observing

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

