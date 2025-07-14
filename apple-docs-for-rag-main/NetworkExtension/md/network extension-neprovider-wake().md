

- Network Extension
- NEProvider
-  wake() 

Instance Method

# wake()

Handle a wake event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func wake()
```

## Discussion

This method is called by the system when the device wakes up from sleep mode.

`NEProvider` subclasses should override this method if the provider needs to perform any tasks when the device wakes up, such as reconnecting a tunnel connection.

## See Also

### Handling sleep and wake

func sleep(completionHandler: () -> Void)

Handle a sleep event.

