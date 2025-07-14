

- Foundation
- NSSet
-  removeObserver(\_:forKeyPath:) 

Instance Method

# removeObserver(\_:forKeyPath:)

Raises an exception.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObserver(
    _ observer: NSObject,
    forKeyPath keyPath: String
)
```

## Parameters 

`observer`  

The object to remove as an observer.

`keyPath`  

A key-path, relative to the set, for which `observer` is registered to receive KVO change notifications. This value must not be `nil`.

## Discussion

`NSSet` objects are not observable, so this method raises an exception when invoked on an `NSSet` object. Instead of observing a set, observe the unordered to-many relationship for which the set is the collection of related objects.

## See Also

### Key-Value Observing

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

