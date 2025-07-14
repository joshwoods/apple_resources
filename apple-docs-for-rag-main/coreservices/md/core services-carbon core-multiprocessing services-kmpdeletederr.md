

- Core Services
- Carbon Core
- Multiprocessing Services
-  kMPDeletedErr 

Global Variable

# kMPDeletedErr

The desired notification the function was waiting upon was deleted.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kMPDeletedErr: Int { get }
```

## See Also

### Result Codes

var kMPIterationEndErr: Int

var kMPPrivilegedErr: Int

var kMPProcessCreatedErr: Int

var kMPProcessTerminatedErr: Int

var kMPTaskCreatedErr: Int

var kMPTaskBlockedErr: Int

The desired task is blocked.

var kMPTaskStoppedErr: Int

The desired task is stopped.

var kMPTimeoutErr: Int

The designated timeout interval passed before the function could take action.

var kMPInsufficientResourcesErr: Int

Could not complete task due to unavailable Multiprocessing Services resources. Note that many functions return this value as a general error when the desired action could not be performed.

var kMPInvalidIDErr: Int

Invalid ID value. For example, an invalid message queue ID was passed to `MPNotifyQueue`.

