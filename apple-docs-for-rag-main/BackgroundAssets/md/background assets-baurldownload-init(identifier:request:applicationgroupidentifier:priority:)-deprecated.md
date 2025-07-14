

- Background Assets
- BAURLDownload
-  init(identifier:request:applicationGroupIdentifier:priority:) Deprecated

Initializer

# init(identifier:request:applicationGroupIdentifier:priority:)

Creates a prioritized download that uses the specified identifier and App Group.

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3Deprecated

``` source
convenience init(
    identifier: String,
    request: URLRequest,
    applicationGroupIdentifier: String,
    priority: BADownload.Priority
)
```

## Parameters 

`identifier`  

An app-specific string that uniquely identifies the downloadable asset.

`request`  

A URL request that provides request-specific information, such as URL, request type, and body data.

`applicationGroupIdentifier`  

The identifier of the App Group where the system stores finished downloads. For more information about App Groups, see Configuring app groups.

`priority`  

The priority of the download. For more information, see BADownload.Priority.

## Discussion

The system requires that all URL requests use Hypertext Transfer Protocol Secure (HTTPS).

## See Also

### Creating a download

init(identifier: String, request: URLRequest, essential: Bool, fileSize: Int, applicationGroupIdentifier: String, priority: BADownload.Priority)

convenience init(identifier: String, request: URLRequest, fileSize: Int, applicationGroupIdentifier: String)

convenience init(identifier: String, request: URLRequest, applicationGroupIdentifier: String)

Creates a download that uses the specified identifier and App Group.

Deprecated

