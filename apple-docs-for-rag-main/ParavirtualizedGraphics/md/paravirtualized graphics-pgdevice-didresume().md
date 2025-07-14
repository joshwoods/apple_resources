

- Paravirtualized Graphics
- PGDevice
-  didResume() 

Instance Method

# didResume()

Tells the device object to finish any remaining work to resume processing of a previously saved device’s suspend state.

Mac Catalyst 14.0+macOS 11.0+

``` source
func didResume()
```

**Required**

## Discussion

After you call this method, the virtualized device can generate new interrupts immediately, even before the call completes. Similarly, guest memory must also be accessible before you call this method.

## See Also

### Suspending and Resuming Graphics Processing

func willSuspend()

Notifies the virtual graphics device to start suspending graphics activities.

**Required**

func finishSuspend() -> Data?

Notifies the virtualized graphics device to finish suspending graphics activities.

**Required**

func willResume(withSuspendState: Data, error: NSErrorPointer) -> Bool

Tells a new device object to load a previously saved device’s suspend state.

**Required**

let PGResumeErrorDomain: String

The error domain for suspend-resume actions.

enum PGResumeErrorCode

Error codes for suspend-resume actions.

