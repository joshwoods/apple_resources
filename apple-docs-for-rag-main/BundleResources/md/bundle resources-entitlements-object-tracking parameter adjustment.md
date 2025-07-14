

- Bundle Resources
- Entitlements
-  Object-tracking parameter adjustment 

Property List Key

# Object-tracking parameter adjustment

A Boolean value that allows an app to use ARKit to track more objects with a higher frequency.

visionOS 2.0+

## Details 

Key  
com.apple.developer.arkit.object-tracking-parameter-adjustment.allow

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

With this entitlement, you can use the ObjectTrackingProvider.TrackingConfiguration to change object tracking parameters.

Note

Object-tracking parameter adjustment is only available in an immersive space. See Setting up access to ARKit data to learn more about opening an immersive space and requesting authorization for ARKit data access. To learn more about best practices for privacy, see Adopting best practices for privacy and user preferences.

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

Spatial barcode and QR code scanning

A Boolean value that indicates whether an app can use ARKit to detect, position, and decode barcode and QR codes.

**Key:** com.apple.developer.arkit.barcode-detection.allow

UVC Device Access on visionOS

A Boolean value that indicates whether the app can stream USB UVC devices connected to the Developer strap.

**Key:** com.apple.developer.avfoundation.uvc-device-access

