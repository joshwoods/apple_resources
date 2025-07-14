

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  releaseHeldCalls() 

Instance Method

# releaseHeldCalls()

Ends all calls that are on hold or returns a busy signal for a waiting call.

macOS 10.7+

``` source
func releaseHeldCalls()
```

## See Also

### Ending Calls

func endCall()

Ends the current call or refuses an incoming call.

func releaseCall(Int32)

Ends the call with the specified index.

func releaseActiveCalls()

Ends all active calls and accepts a held or waiting call.

