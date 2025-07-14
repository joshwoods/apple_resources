

- Foundation
- NSExtensionContext
-  open(\_:completionHandler:) 

Instance Method

# open(\_:completionHandler:)

Asks the system to open a URL on behalf of the currently running app extension.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func open(
    _ URL: URL,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func open(_ URL: URL) async -> Bool
```

## Parameters 

`URL`  

The URL to open.

`completionHandler`  

A block/closure to be called when the URL has opened. The closure takes a single boolean parameter indicating whether the operation was successful.

## Discussion

Each extension point determines whether to support this method, or under which conditions to support this method. In iOS, the Today and iMessage app extension points support this method. An iMessage app extension can use this method only to open its parent app, and only if the parent app is shown on the iOS home screen.

Important

You can use this method in a Today widget to open the widget’s containing app. If you use this method to open other apps from your Today widget, your App Store submission may require additional review. To learn more, see App Store Review Guidelines and iOS Human Interface Guidelines.

