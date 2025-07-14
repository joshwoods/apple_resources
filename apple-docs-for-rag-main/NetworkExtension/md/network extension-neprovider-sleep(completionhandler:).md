

- Network Extension
- NEProvider
-  sleep(completionHandler:) 

Instance Method

# sleep(completionHandler:)

Handle a sleep event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func sleep(completionHandler: @escaping () -> Void)
```

``` source
func sleep() async
```

## Parameters 

`completionHandler`  

Implementations of this method must execute this block when the provider is finished handling the sleep event.

## Discussion

This method is called by the system when the device is about to go to sleep.

`NEProvider` subclasses should override this method if the provider needs to perform any tasks before the device sleeps, such as disconnecting a tunnel connection.

## See Also

### Handling sleep and wake

func wake()

Handle a wake event.

