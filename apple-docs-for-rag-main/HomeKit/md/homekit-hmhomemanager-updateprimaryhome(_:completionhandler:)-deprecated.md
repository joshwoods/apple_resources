

- HomeKit
- HMHomeManager
-  updatePrimaryHome(\_:completionHandler:) Deprecated

Instance Method

# updatePrimaryHome(\_:completionHandler:)

Updates the primary home of this home manager.

iOS 8.0–16.1DeprecatediPadOS 8.0–16.1DeprecatedMac Catalyst 13.1–16.1DeprecatedtvOS 10.0–16.1DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–9.1Deprecated

``` source
func updatePrimaryHome(
    _ home: HMHome,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updatePrimaryHome(_ home: HMHome) async throws
```

Deprecated

This method is no longer supported.

## Parameters 

`home`  

The new primary home. Must be a home managed by this home manager.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Managing the primary home

var primaryHome: HMHome?

The primary home managed by this home manager.

Deprecated

