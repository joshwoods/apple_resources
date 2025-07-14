

- Screen Time
- STWebHistory
-  init(bundleIdentifier:) 

Initializer

# init(bundleIdentifier:)

Creates a web history instance to delete web-usage data associated to the bundle identifier you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
init(bundleIdentifier: String) throws
```

## Parameters 

`bundleIdentifier`  

The bundle identifier.

## Discussion

The default value for `bundleIdentifier` is `Bundle.main.bundleIdentifier`. This is the recommended identifier to use, except for example, if a helper process is presenting web UI and you want to group that web-usage under the main app’s bundle identifier.

