

- Foundation
- Operation
-  qualityOfService 

Instance Property

# qualityOfService

The relative amount of importance for granting system resources to the operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var qualityOfService: QualityOfService { get set }
```

## Discussion

Service levels affect the priority with which an operation object is given access to system resources such as CPU time, network resources, disk resources, and so on. Operations with a higher quality of service level are given greater priority over system resources so that they may perform their task more quickly. You use service levels to ensure that operations responding to explicit user requests are given priority over less critical work.

This property reflects the minimum service level needed to execute the operation effectively. The default value of this property is QualityOfService.default and you should leave that value in place whenever possible. When changing the service level, use the minimum level that is appropriate for executing the corresponding task. For example, if the user initiates a task and is waiting for it to finish, assign the value QualityOfService.userInteractive to this property. The system may give the operation a higher service level to the operation if the resources are available to do so. For additional information, see Prioritize Work with Quality of Service Classes in Energy Efficiency Guide for iOS Apps and Prioritize Work at the Task Level in Energy Efficiency Guide for Mac Apps.

## See Also

### Configuring the Execution Priority

var threadPriority: Double

The thread priority to use when executing the operation

Deprecated

var queuePriority: Operation.QueuePriority

The execution priority of the operation in an operation queue.

