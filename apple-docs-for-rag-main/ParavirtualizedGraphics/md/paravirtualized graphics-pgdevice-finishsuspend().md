

- Paravirtualized Graphics
- PGDevice
-  finishSuspend() 

Instance Method

# finishSuspend()

Notifies the virtualized graphics device to finish suspending graphics activities.

Mac Catalyst 14.0+macOS 11.0+

``` source
func finishSuspend() -> Data?
```

**Required**

## Return Value

The suspend state data, or `nil` if an error occurred.

## Discussion

This method may take an arbitrary amount of time as the device needs to complete any unfinished GPU work. After this call completes, you can’t perform any further operations on this device object and must release it.

Typically, your app serializes the suspend state data to persistant storage. Pass the suspend state data to a new device object when you want to resume graphics operations.

## See Also

### Suspending and Resuming Graphics Processing

func willSuspend()

Notifies the virtual graphics device to start suspending graphics activities.

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

