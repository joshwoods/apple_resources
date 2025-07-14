

- Paravirtualized Graphics
- PGDevice
-  willSuspend() 

Instance Method

# willSuspend()

Notifies the virtual graphics device to start suspending graphics activities.

Mac Catalyst 14.0+macOS 11.0+

``` source
func willSuspend()
```

**Required**

## Discussion

The virtualized device stops generating interrupts and won’t accept new commands from the guest. You must halt any guest CPUs within a short interval after you call this method.

## See Also

### Suspending and Resuming Graphics Processing

func finishSuspend() -> Data?

Notifies the virtualized graphics device to finish suspending graphics activities.

**Required**

func willResume(withSuspendState: Data, error: NSErrorPointer) -> Bool

Tells a new device object to load a previously saved device’s suspend state.

**Required**

func didResume()

Tells the device object to finish any remaining work to resume processing of a previously saved device’s suspend state.

**Required**

let PGResumeErrorDomain: String

The error domain for suspend-resume actions.

enum PGResumeErrorCode

Error codes for suspend-resume actions.

