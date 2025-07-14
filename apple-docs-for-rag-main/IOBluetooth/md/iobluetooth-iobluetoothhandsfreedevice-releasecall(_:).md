

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  releaseCall(\_:) 

Instance Method

# releaseCall(\_:)

Ends the call with the specified index.

macOS 10.7+

``` source
func releaseCall(_ index: Int32)
```

## Parameters 

`index`  

The index of the call to end.

## See Also

### Ending Calls

func endCall()

Ends the current call or refuses an incoming call.

func releaseActiveCalls()

Ends all active calls and accepts a held or waiting call.

func releaseHeldCalls()

Ends all calls that are on hold or returns a busy signal for a waiting call.

