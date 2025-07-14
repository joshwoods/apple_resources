

- XCTest
- XCTAttachment
-  init(data:uniformTypeIdentifier:) 

Initializer

# init(data:uniformTypeIdentifier:)

Creates an attachment containing the provided data payload, with a custom UTI.

``` source
convenience init(
    data payload: Data,
    uniformTypeIdentifier identifier: String
)
```

## Parameters 

`payload`  

The data to wrap as an attachment.

`identifier`  

A custom UTI to represent the data’s content type.

## Discussion

Creates an attachment with a uniformTypeIdentifier of ``` "``public.data" ```.

## See Also

### Creating Attachments from Data

convenience init(data: Data)

Creates an attachment containing the provided data payload.

init(uniformTypeIdentifier: String?, name: String?, payload: Data?, userInfo: [AnyHashable : Any]?)

Creates an attachment containing the provided data payload, optionally with a custom UTI, name, and user-provided metadata dictionary.

