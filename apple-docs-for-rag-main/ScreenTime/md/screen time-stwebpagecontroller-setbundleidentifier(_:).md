

- Screen Time
- STWebpageController
-  setBundleIdentifier(\_:) 

Instance Method

# setBundleIdentifier(\_:)

Changes the bundle identifier used to report web usage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor
func setBundleIdentifier(_ bundleIdentifier: String) throws
```

## Parameters 

`bundleIdentifier`  

The bundle identifier that can be changed to facilitate web usage reporting for a parent web browser from one of its helper processes or extensions.

## Discussion

This is only supported for web browsers that have been properly registered with Screen Time.

