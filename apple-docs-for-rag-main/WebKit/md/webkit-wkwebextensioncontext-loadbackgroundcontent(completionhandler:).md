

- WebKit
- WKWebExtensionContext
-  loadBackgroundContent(completionHandler:) 

Instance Method

# loadBackgroundContent(completionHandler:)

Loads the background content if needed for the extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func loadBackgroundContent(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
@MainActor
func loadBackgroundContent() async throws
```

## Parameters 

`completionHandler`  

A block to be called upon completion of the loading process, with an optional error.

## Discussion

This method forces the loading of the background content for the extension that will otherwise be loaded on-demand during specific events.

It is useful when the app requires the background content to be loaded for other reasons. If the background content is already loaded, the completion handler will be called immediately. An error will occur if the extension does not have any background content to load or loading fails.

