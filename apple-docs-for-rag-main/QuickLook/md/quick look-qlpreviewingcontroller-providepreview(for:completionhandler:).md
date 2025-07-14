

- Quick Look
- QLPreviewingController
-  providePreview(for:completionHandler:) 

Instance Method

# providePreview(for:completionHandler:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
optional func providePreview(
    for request: QLFilePreviewRequest,
    completionHandler handler: @escaping (QLPreviewReply?, (any Error)?) -> Void
)
```

``` source
optional func providePreview(for request: QLFilePreviewRequest) async throws -> QLPreviewReply
```

