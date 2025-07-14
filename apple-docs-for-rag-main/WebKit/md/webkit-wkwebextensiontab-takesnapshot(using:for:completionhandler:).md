

- WebKit
- WKWebExtensionTab
-  takeSnapshot(using:for:completionHandler:) 

Instance Method

# takeSnapshot(using:for:completionHandler:)

Called to capture a snapshot of the current webpage as an image.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
optional func takeSnapshot(
    using configuration: WKSnapshotConfiguration,
    for context: WKWebExtensionContext,
    completionHandler: @escaping (UIImage?, (any Error)?) -> Void
)
```

**macOS**

``` source
@MainActor
optional func takeSnapshot(
    using configuration: WKSnapshotConfiguration,
    for context: WKWebExtensionContext,
    completionHandler: @escaping (NSImage?, (any Error)?) -> Void
)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
optional func snapshot(
    using configuration: WKSnapshotConfiguration,
    for context: WKWebExtensionContext
) async throws -> UIImage?
```

**macOS**

``` source
@MainActor
optional func snapshot(
    using configuration: WKSnapshotConfiguration,
    for context: WKWebExtensionContext
) async throws -> NSImage?
```

## Parameters 

`configuration`  

An object that specifies how the snapshot is configured.

`context`  

The context in which the web extension is running.

`completionHandler`  

A block that must be called upon completion. The block takes two arguments: the captured image of the webpage (or `nil` if capturing failed) and an error, which should be provided if any errors occurred.

## Discussion

Defaults to capturing the visible area of the tab’s web view if not implemented.

