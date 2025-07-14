

- XCTest
- XCTAttachment
-  init(uniformTypeIdentifier:name:payload:userInfo:) 

Initializer

# init(uniformTypeIdentifier:name:payload:userInfo:)

Creates an attachment containing the provided data payload, optionally with a custom UTI, name, and user-provided metadata dictionary.

``` source
init(
    uniformTypeIdentifier identifier: String?,
    name: String?,
    payload: Data?,
    userInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`identifier`  

An optional custom UTI to represent the data’s content type.

`name`  

An optional name for the attachment, to be used in Xcode’s test reports.

`payload`  

The data to wrap as an attachment.

`userInfo`  

An optional dictionary of user-provided metadata to associate with the attachment.

## Discussion

Creates an attachment with a uniformTypeIdentifier of `"public.data"` if the `identifier` parameter is `nil`.

## See Also

### Creating Attachments from Data

convenience init(data: Data)

Creates an attachment containing the provided data payload.

convenience init(data: Data, uniformTypeIdentifier: String)

Creates an attachment containing the provided data payload, with a custom UTI.

