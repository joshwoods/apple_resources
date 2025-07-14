

- Matter
- MTRBaseClusterWiFiNetworkManagement
-  networkPassphraseRequest(with:completion:) 

Instance Method

# networkPassphraseRequest(with:completion:)

Command NetworkPassphraseRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func networkPassphraseRequest(
    with params: MTRWiFiNetworkManagementClusterNetworkPassphraseRequestParams?,
    completion: @escaping (MTRWiFiNetworkManagementClusterNetworkPassphraseResponseParams?, (any Error)?) -> Void
)
```

``` source
func networkPassphraseRequest(with params: MTRWiFiNetworkManagementClusterNetworkPassphraseRequestParams?) async throws -> MTRWiFiNetworkManagementClusterNetworkPassphraseResponseParams
```

## Discussion

Request the current WPA-Personal passphrase or PSK associated with the managed Wi-Fi network.

