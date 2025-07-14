

- HomeKit
- HMCharacteristic
-  readValue(completionHandler:) 

Instance Method

# readValue(completionHandler:)

Reads the value for the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
func readValue(completionHandler completion: @escaping ((any Error)?) -> Void)
```

``` source
func readValue() async throws
```

## Parameters 

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

The value is available from the value property after completion of the request.

## See Also

### Controlling a characteristic

var value: Any?

The current value of the characteristic.

func writeValue(Any?, completionHandler: ((any Error)?) -> Void)

Modifies the value of the characteristic.

func updateAuthorizationData(Data?, completionHandler: ((any Error)?) -> Void)

Sets or clears authorization data used when writing to the characteristic.

