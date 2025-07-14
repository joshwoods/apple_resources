

- Local Authentication
- LAContext
-  biometryType 

Instance Property

# biometryType

The type of biometric authentication supported by the device.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13.2+visionOS 1.0+watchOS 11.0+

``` source
var biometryType: LABiometryType { get }
```

## Discussion

Use the value of this property to ensure that any authentication-related user prompts you create match the biometric capabilities of the device. For example, if the value of this property is LABiometryType.faceID, don’t refer to Touch ID in an authentication prompt.

This property is set only after you call the canEvaluatePolicy(_:error:) method, and is set no matter what the call returns. The default value is LABiometryType.none.

## See Also

### Checking availability

func canEvaluatePolicy(LAPolicy, error: NSErrorPointer) -> Bool

Assesses whether authentication can proceed for a given policy.

enum LAPolicy

The set of available local authentication policies.

enum LABiometryType

The set of available biometric authentication types.

