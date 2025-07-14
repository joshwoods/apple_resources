

- Bundle Resources
- Entitlements
-  Persistent Content Capture 

Property List Key

# Persistent Content Capture

A Boolean value that indicates whether a Virtual Network Computing (VNC) app needs persistent access to screen capture.

macOS 14.4+

## Details 

Key  
com.apple.developer.persistent-content-capture

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

The Persistent Content Capture entitlement enables VNC apps to view and record the screen.

Before your app can use this entitlement, request permission to use it by submitting the Persistent Content Capture Entitlement Request form. After receiving permission from Apple to use this entitlement, add it to your app’s profile in Xcode following the instrucitons Apple provides.

