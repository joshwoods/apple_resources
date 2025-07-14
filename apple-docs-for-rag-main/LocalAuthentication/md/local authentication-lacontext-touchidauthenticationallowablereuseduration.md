

- Local Authentication
- LAContext
-  touchIDAuthenticationAllowableReuseDuration 

Instance Property

# touchIDAuthenticationAllowableReuseDuration

The duration for which Touch ID authentication reuse is allowable.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
var touchIDAuthenticationAllowableReuseDuration: TimeInterval { get set }
```

## Discussion

If the user unlocks the device using Touch ID within the specified time interval, then authentication for the receiver succeeds automatically, without prompting the user for Touch ID. This bypasses a scenario where the user unlocks the device and then is almost immediately prompted for another fingerprint.

The default value is `0`, meaning that Touch ID authentication isn’t reused.

The maximum allowable duration for Touch ID authentication reuse is specified by the LATouchIDAuthenticationMaximumAllowableReuseDuration constant. You cannot specify a longer duration by setting this property to a value greater than this constant.

## See Also

### Reusing device unlock state

let LATouchIDAuthenticationMaximumAllowableReuseDuration: TimeInterval

The maximum allowable reuse duration.

