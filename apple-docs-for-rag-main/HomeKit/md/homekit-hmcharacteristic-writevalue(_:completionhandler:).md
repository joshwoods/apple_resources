

- HomeKit
- HMCharacteristic
-  writeValue(\_:completionHandler:) 

Instance Method

# writeValue(\_:completionHandler:)

Modifies the value of the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
func writeValue(
    _ value: Any?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func writeValue(_ value: Any?) async throws
```

## Parameters 

`value`  

The new value.

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

func updateAuthorizationData(Data?, completionHandler: ((any Error)?) -> Void)

Sets or clears authorization data used when writing to the characteristic.

