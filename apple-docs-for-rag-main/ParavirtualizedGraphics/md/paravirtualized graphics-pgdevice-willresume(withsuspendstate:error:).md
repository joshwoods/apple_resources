

- Paravirtualized Graphics
- PGDevice
-  willResume(withSuspendState:error:) 

Instance Method

# willResume(withSuspendState:error:)

Tells a new device object to load a previously saved device’s suspend state.

Mac Catalyst 14.0+macOS 11.0+

``` source
func willResume(
    withSuspendState suspendState: Data,
    error: NSErrorPointer
) -> Bool
```

**Required**

## Parameters 

`suspendState`  

The suspend data that you previously saved when you suspended an earlier device object.

## Return Value

A Boolean value that indicates whether the framework was able to start restoring the graphics data.

## Discussion

This method sets up the device to appear in the same state it was in before the suspend. The device object doesn’t access guest memory during the call to this method.

When resuming from an earlier suspended device, this must be the first method that you call on the newly created device object. When you call this method, ensure that the guest CPUs aren’t running.

After you call this method, reattach any suspended displays before calling didResume().

## See Also

### Suspending and Resuming Graphics Processing

func willSuspend()

Notifies the virtual graphics device to start suspending graphics activities.

**Required**

func finishSuspend() -> Data?

Notifies the virtualized graphics device to finish suspending graphics activities.

**Required**

func didResume()

Tells the device object to finish any remaining work to resume processing of a previously saved device’s suspend state.

**Required**

let PGResumeErrorDomain: String

The error domain for suspend-resume actions.

enum PGResumeErrorCode

Error codes for suspend-resume actions.

