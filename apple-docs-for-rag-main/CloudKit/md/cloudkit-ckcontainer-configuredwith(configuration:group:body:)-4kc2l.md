

- CloudKit
- CKContainer
-  configuredWith(configuration:group:body:) 

Instance Method

# configuredWith(configuration:group:body:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@discardableResult @preconcurrency
func configuredWith(
    configuration: CKOperation.Configuration? = nil,
    group: CKOperationGroup? = nil,
    body: (CKContainer) async throws -> R
) async rethrows -> R
```

