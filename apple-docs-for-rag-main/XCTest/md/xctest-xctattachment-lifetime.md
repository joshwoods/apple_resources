

- XCTest
- XCTAttachment
-  lifetime 

Instance Property

# lifetime

Indicates whether the attachment is kept or discarded when its associated test passes.

``` source
var lifetime: XCTAttachment.Lifetime { get set }
```

## Mentioned in 

Adding Attachments to Tests, Activities, and Issues

## Discussion

Defaults to XCTAttachment.Lifetime.deleteOnSuccess, indicating that the attachment should be discarded when its test passes successfully, to save on storage space. Set this property to XCTAttachment.Lifetime.keepAlways to persist an attachment even when its test passes.

## See Also

### Setting an Attachment’s Lifetime

enum Lifetime

The possible lifetime values for a test attachment.

