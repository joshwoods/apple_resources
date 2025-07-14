

- Background Assets
- BADownloadManager
-  shared 

Type Property

# shared

The download manager that both the app and the extension share.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
class var shared: BADownloadManager { get }
```

## Discussion

Because the download manager is a shared resource, use the withExclusiveControl(_:) or withExclusiveControl(beforeDate:perform:) methods to acquire exclusive control of the manager before you use it to access, schedule, or cancel downloads.

