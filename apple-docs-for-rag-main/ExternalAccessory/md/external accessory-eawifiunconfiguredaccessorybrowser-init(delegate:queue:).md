

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowser
-  init(delegate:queue:) 

Initializer

# init(delegate:queue:)

Creates a browser object that scans for unconfigured accessories.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    delegate: (any EAWiFiUnconfiguredAccessoryBrowserDelegate)?,
    queue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

The object that you use to receive browser-related events.

`queue`  

The dispatch queue on which the delegate would like to receive events. If `nil`, the events will be on the main queue.

## Return Value

An initialized browser object.

## Discussion

This method is the designated initializer for `EAWiFiUnconfiguredAccessoryBrowser`. After initialization, an app can configure a browser object based on its interests.

