

- Paravirtualized Graphics
-  PGResumeErrorDomain 

Global Variable

# PGResumeErrorDomain

The error domain for suspend-resume actions.

Mac Catalyst 14.0+macOS 11.0+

``` source
let PGResumeErrorDomain: String
```

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

func didResume()

Tells the device object to finish any remaining work to resume processing of a previously saved device’s suspend state.

**Required**

enum PGResumeErrorCode

Error codes for suspend-resume actions.

