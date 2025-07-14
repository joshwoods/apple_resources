

- Foundation
- NSArray
-  removeObserver(\_:fromObjectsAt:forKeyPath:) 

Instance Method

# removeObserver(\_:fromObjectsAt:forKeyPath:)

Removes `anObserver` from all key value observer notifications associated with the specified `keyPath` relative to the array’s objects at `indexes`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeObserver(
    _ observer: NSObject,
    fromObjectsAt indexes: IndexSet,
    forKeyPath keyPath: String
)
```

## Parameters 

`observer`  

The observer.

`indexes`  

The index set.

`keyPath`  

The key path, relative to the array, to be observed.

## Discussion

This is not merely a convenience method; invoking this method is potentially much faster than repeatedly invoking removeObserver(_:forKeyPath:).

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

func addObserver(NSObject, toObjectsAt: IndexSet, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Registers an observer to receive key value observer notifications for the specified key-path relative to the objects at the indexes.

