

- Core Location
- CLLocationPushServiceExtension
-  serviceExtensionWillTerminate() 

Instance Method

# serviceExtensionWillTerminate()

Notifies your app extension that the system is about to terminate the extension because it’s taking too long to complete its task.

iOS 15.0+iPadOS 15.0+

``` source
optional func serviceExtensionWillTerminate()
```

## Discussion

If your didReceiveLocationPushPayload(_:completion:) method takes too long to collect a location and call its completion block, the system calls this method on the main thread. Use this method to execute the completion block from didReceiveLocationPushPayload(_:completion:) as quickly as possible.

