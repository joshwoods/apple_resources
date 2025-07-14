

- Background Assets
- BAURLDownload
-  init(identifier:request:fileSize:applicationGroupIdentifier:) 

Initializer

# init(identifier:request:fileSize:applicationGroupIdentifier:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 18.4+visionOS 2.4+

``` source
convenience init(
    identifier: String,
    request: URLRequest,
    fileSize: Int,
    applicationGroupIdentifier: String
)
```

## See Also

### Creating a download

init(identifier: String, request: URLRequest, essential: Bool, fileSize: Int, applicationGroupIdentifier: String, priority: BADownload.Priority)

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String)

Creates a download that uses the specified identifier and App Group.

Deprecated

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String, priority: BADownload.Priority)

Creates a prioritized download that uses the specified identifier and App Group.

Deprecated

