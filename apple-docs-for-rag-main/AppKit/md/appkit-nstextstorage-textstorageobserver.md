

- AppKit
- NSTextStorage
-  textStorageObserver 

Instance Property

# textStorageObserver

The observer for the text storage object.

macOS 12.0+

``` source
weak var textStorageObserver: (any NSTextStorageObserving)? { get set }
```

## See Also

### Accessing the storage controller

protocol NSTextStorageObserving

Optional methods that delegates implement to handle editing and transaction processing.

