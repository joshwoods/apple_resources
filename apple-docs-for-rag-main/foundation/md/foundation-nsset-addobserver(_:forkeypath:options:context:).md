

- Foundation
- NSSet
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

The key path, relative to the set, of the property to observe. This value must not be `nil`.

`options`  

A combination of the NSKeyValueObservingOptions values that specifies what is included in observation notifications. For possible values, see NSKeyValueObservingOptions.

`context`  

Arbitrary data that is passed to `observer` in observeValue(forKeyPath:of:change:context:).

## Discussion

`NSSet` objects are not observable, so this method raises an exception when invoked on an `NSSet` object. Instead of observing a set, observe the unordered to-many relationship for which the set is the collection of related objects.

## See Also

### Key-Value Observing

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

