

- HomeKit
- HMCharacteristic
-  updateAuthorizationData(\_:completionHandler:) 

Instance Method

# updateAuthorizationData(\_:completionHandler:)

Sets or clears authorization data used when writing to the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateAuthorizationData(
    _ data: Data?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateAuthorizationData(_ data: Data?) async throws
```

## Parameters 

`data`  

New authorization data to use. Pass `nil` to remove authorization data.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Controlling a characteristic

var value: Any?

The current value of the characteristic.

func readValue(completionHandler: ((any Error)?) -> Void)

Reads the value for the characteristic.

func writeValue(Any?, completionHandler: ((any Error)?) -> Void)

Modifies the value of the characteristic.

