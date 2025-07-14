

- Objective-C Runtime
- NSObject
-  removeObserver(\_:forKeyPath:) 

Instance Method

# removeObserver(\_:forKeyPath:)

Stops the observer object from receiving change notifications for the property specified by the key path relative to the object receiving this message.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

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

A key-path, relative to the object receiving this message, for which `observer` is registered to receive KVO change notifications.

## Discussion

It is an error to call removeObserver(_:forKeyPath:) for an `object` that has not previously been registered as an observer.

Be sure to invoke this method (or removeObserver(_:forKeyPath:context:)) before any object specified in addObserver(_:forKeyPath:options:context:) is deallocated.

## See Also

### Registering for Observation

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Registers the observer object to receive KVO notifications for the key path relative to the object receiving this message.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Stops the observer object from receiving change notifications for the property specified by the key path relative to the object receiving this message, given the context.

