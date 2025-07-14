

- Matter
- MTRDeviceAttestationDelegate
-  deviceAttestation(\_:completedForDevice:attestationDeviceInfo:error:) Deprecated

Instance Method

# deviceAttestation(\_:completedForDevice:attestationDeviceInfo:error:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
optional func deviceAttestation(
    _ controller: MTRDeviceController,
    completedForDevice device: UnsafeMutableRawPointer,
    attestationDeviceInfo: MTRDeviceAttestationDeviceInfo,
    error: (any Error)?
)
```

Deprecated

Please implement deviceAttestationCompletedForController:opaqueDeviceHandle:attestationDeviceInfo:error:

