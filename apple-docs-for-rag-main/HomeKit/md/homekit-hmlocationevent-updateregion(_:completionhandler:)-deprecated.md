

- HomeKit
- HMLocationEvent
-  updateRegion(\_:completionHandler:) Deprecated

Instance Method

# updateRegion(\_:completionHandler:)

Changes the region associated with this event.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
func updateRegion(
    _ region: CLRegion,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

**Mac Catalyst**

``` source
func updateRegion(_ region: CLRegion) async throws
```

Deprecated

Use the mutable region property on the HMMutableLocationEvent subclass of HMLocationEvent instead.

## Parameters 

`region`  

New region on which the event is triggered. Must have at least one of notifyOnEntry or notifyOnExit set to true.

`completion`  

The block executed when the region update request has been processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

