

- Network Extension
- NEHotspotNetwork
-  fetchCurrent(completionHandler:) 

Type Method

# fetchCurrent(completionHandler:)

Fetches information about the current Wi-Fi network.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func fetchCurrent(completionHandler: @escaping (NEHotspotNetwork?) -> Void)
```

``` source
class func fetchCurrent() async -> NEHotspotNetwork?
```

## Parameters 

`completionHandler`  

A Swift closure or an ObjectiveC block that receives an NEHotspotNetwork instance that contains the current SSID, BSSID, and security type. This call doesn’t populate other fields in the object. The block executes on the main thread and only after the call obtains the current Wi-Fi parameters from the system. If any of the criteria discussed below aren’t fulfilled, the `currentNetwork` parameter received by completion handler is `nil`.

## Discussion

This method produces a non-`nil` NEHotspotNetwork object only when the requesting app meets at least one of the following criteria:

- The app is using the Core Location API and has user’s authorization to access precise location.

- The app used the NEHotspotConfiguration API to configure the current Wi-Fi network.

- The app has active VPN configurations installed.

- The app has an active NEDNSSettingsManager configuration installed.

This method also requires the app to have the Access Wi-Fi Information Entitlement, and produces `nil` if the app lacks this entitlement.

