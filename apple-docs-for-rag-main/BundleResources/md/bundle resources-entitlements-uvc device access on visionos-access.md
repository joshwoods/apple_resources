

- Bundle Resources
- Entitlements
-  UVC Device Access on visionOS 

Property List Key

# UVC Device Access on visionOS

A Boolean value that indicates whether the app can stream USB UVC devices connected to the Developer strap.

visionOS 2.1+

## Details 

Key  
com.apple.developer.avfoundation.uvc-device-access

Type  

boolean

## Discussion

On visionOS, your app must have the this entitlement to discover and use devices of type external using an AVCaptureDevice.DiscoverySession.

This feature only supports USB2 devices drawing a maximum 500mA and supports the use of up to 1 hub.

## See Also

### Enterprise

Apple Neural Engine access

A Boolean value that indicates whether an app can use the Apple Neural Engine to speed up CoreML.

**Key:** com.apple.developer.coreml.neural-engine-access

Increased performance headroom

An entitlement that allows an app to adjust thresholds that balance thermal dissipation and performance against fan noise and other factors.

**Key:** com.apple.developer.app-compute-category

Passthrough in screen capture

A Boolean value that indicates whether an app can include passthrough in screen capture.

**Key:** com.apple.developer.screen-capture.include-passthrough

Main camera access

A Boolean value that indicates whether an app can use ARKit to access the main cameras on Apple Vision Pro.

**Key:** com.apple.developer.arkit.main-camera-access.allow

Object-tracking parameter adjustment

A Boolean value that allows an app to use ARKit to track more objects with a higher frequency.

**Key:** com.apple.developer.arkit.object-tracking-parameter-adjustment.allow

Spatial barcode and QR code scanning

A Boolean value that indicates whether an app can use ARKit to detect, position, and decode barcode and QR codes.

**Key:** com.apple.developer.arkit.barcode-detection.allow

