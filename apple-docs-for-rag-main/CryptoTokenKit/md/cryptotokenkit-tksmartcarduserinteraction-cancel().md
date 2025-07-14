

- CryptoTokenKit
- TKSmartCardUserInteraction
-  cancel() 

Instance Method

# cancel()

Attempts to cancel an interaction started by calling run(reply:). For certain interactions, cancellation may not be available.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
func cancel() -> Bool
```

## Return Value

Returns false if the operation is not running, or if cancelation is not supported.

## See Also

### Starting and Stopping

func run(reply: (Bool, (any Error)?) -> Void)

Runs the user interaction and asynchronously receives a reply.

