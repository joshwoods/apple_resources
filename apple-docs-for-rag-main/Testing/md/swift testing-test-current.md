

- Swift Testing
- Test
-  current 

Type Property

# current

The test that is running on the current task, if any.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static var current: Test? { get }
```

## Discussion

If the current task is running a test, or is a subtask of another task that is running a test, the value of this property describes that test. If no test is currently running, the value of this property is `nil`.

If the current task is detached from a task that started running a test, or if the current thread was created without using Swift concurrency (e.g. by using Thread.detachNewThread(_:) or DispatchQueue.async(execute:)), the value of this property may be `nil`.

