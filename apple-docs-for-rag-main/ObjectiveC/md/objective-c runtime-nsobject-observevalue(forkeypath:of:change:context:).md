

- Objective-C Runtime
- NSObject
-  observeValue(forKeyPath:of:change:context:) 

Instance Method

# observeValue(forKeyPath:of:change:context:)

Informs the observing object when the value at the specified key path relative to the observed object has changed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func observeValue(
    forKeyPath keyPath: String?,
    of object: Any?,
    change: [NSKeyValueChangeKey : Any]?,
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`keyPath`  

The key path, relative to `object`, to the value that has changed.

`object`  

The source object of the key path `keyPath`.

`change`  

A dictionary that describes the changes that have been made to the value of the property at the key path `keyPath` relative to `object`. Entries are described in `Change Dictionary Keys`.

`context`  

The value that was provided when the observer was registered to receive key-value observation notifications.

## Discussion

For an `object` to begin sending change notification messages for the value at `keyPath`, you send it an addObserver(_:forKeyPath:options:context:) message, naming the observing object that should receive the messages. When you are done observing, and in particular before the observing object is deallocated, you send the observed object a removeObserver(_:forKeyPath:) or removeObserver(_:forKeyPath:context:) message to unregister the observer, and stop sending change notification messages.

