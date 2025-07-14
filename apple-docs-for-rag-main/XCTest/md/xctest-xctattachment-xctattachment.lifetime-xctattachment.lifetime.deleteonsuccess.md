

- XCTest
- XCTAttachment
- XCTAttachment.Lifetime
-  XCTAttachment.Lifetime.deleteOnSuccess 

Case

# XCTAttachment.Lifetime.deleteOnSuccess

Indicates that the attachment should be deleted if the test passes.

``` source
case deleteOnSuccess
```

## Mentioned in 

Adding Attachments to Tests, Activities, and Issues

## Discussion

XCTAttachment.Lifetime.deleteOnSuccess is the default lifetime for all new attachments. This lifetime indicates that an attachment should be discarded if its test passes successfully, to save on storage space.

To persist an attachment even when its test passes, set the attachment’s lifetime property to XCTAttachment.Lifetime.keepAlways after attachment initialization.

## See Also

### Attachment Lifetimes

case keepAlways

Indicates that the attachment should be persisted as part of the test’s results even if the test passes.

