

- ARKit
- ARAppClipCodeAnchor
-  radius 

Instance Property

# radius

The App Clip Code’s radius in meters.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+

``` source
var radius: Float { get }
```

## Discussion

ARKit estimates the value of this property at runtime. As the user views an App Clip Code from different angles, ARKit refines its estimate of the true radius of the App Clip Code.

