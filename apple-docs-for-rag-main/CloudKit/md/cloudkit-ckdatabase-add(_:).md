

- CloudKit
- CKDatabase
-  add(\_:) 

Instance Method

# add(\_:)

Executes the specified operation in the current database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
func add(_ operation: CKDatabaseOperation)
```

## Parameters 

`operation`  

The operation to execute.

## Discussion

Configure the operation fully before you call this method. Prior to the operation executing, CloudKit sets its database property to the current database. The operation executes at the priority and quality of service (QoS) that you specify using the queuePriority and qualityOfService properties.

