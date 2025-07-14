

- XCTest
- XCTAttachment
-  init(data:) 

Initializer

# init(data:)

Creates an attachment containing the provided data payload.

``` source
convenience init(data payload: Data)
```

## Parameters 

`payload`  

The data to wrap as an attachment.

## Discussion

Creates an attachment with a uniformTypeIdentifier of ``` "``public.data" ```.

## See Also

### Creating Attachments from Data

convenience init(data: Data, uniformTypeIdentifier: String)

Creates an attachment containing the provided data payload, with a custom UTI.

init(uniformTypeIdentifier: String?, name: String?, payload: Data?, userInfo: [AnyHashable : Any]?)

Creates an attachment containing the provided data payload, optionally with a custom UTI, name, and user-provided metadata dictionary.

