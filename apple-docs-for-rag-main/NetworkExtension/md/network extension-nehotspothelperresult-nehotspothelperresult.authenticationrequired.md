

- Network Extension
- NEHotspotHelperResult
-  NEHotspotHelperResult.authenticationRequired 

Case

# NEHotspotHelperResult.authenticationRequired

The network requires authentication again. This result is only valid in response to a command with type NEHotspotHelperCommandType.maintain.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case authenticationRequired
```

## See Also

### Results

case success

The command was handled successfully.

case failure

The command failed to be handled.

case uiRequired

The operation requires user interaction. This result is only valid in response to a command with type NEHotspotHelperCommandType.authenticate.

case commandNotRecognized

The helper did not recognize the command type.

case unsupportedNetwork

After attempting to authenticate, the Hotspot Helper app determined that it can’t perform the authentication. This result is only valid in response to commands of type NEHotspotHelperCommandType.authenticate and NEHotspotHelperCommandType.presentUI.

case temporaryFailure

The Hotspot Helper app determined that it is temporarily unable to perform the authentication. This result is only valid in response to commands of type NEHotspotHelperCommandType.authenticate and NEHotspotHelperCommandType.presentUI.

