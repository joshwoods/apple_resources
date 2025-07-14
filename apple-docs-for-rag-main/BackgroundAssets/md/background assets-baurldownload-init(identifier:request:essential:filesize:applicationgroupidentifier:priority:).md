

- Background Assets
- BAURLDownload
-  init(identifier:request:essential:fileSize:applicationGroupIdentifier:priority:) 

Initializer

# init(identifier:request:essential:fileSize:applicationGroupIdentifier:priority:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 18.4+visionOS 2.4+

``` source
init(
    identifier: String,
    request: URLRequest,
    essential: Bool,
    fileSize: Int,
    applicationGroupIdentifier: String,
    priority: BADownload.Priority
)
```

## See Also

### Creating a download

convenience init(identifier: String, request: URLRequest, fileSize: Int, applicationGroupIdentifier: String)

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String)

Creates a download that uses the specified identifier and App Group.

Deprecated

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String, priority: BADownload.Priority)

Creates a prioritized download that uses the specified identifier and App Group.

Deprecated

