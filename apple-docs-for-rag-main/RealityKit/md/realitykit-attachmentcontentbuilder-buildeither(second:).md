

- RealityKit
- AttachmentContentBuilder
-  buildEither(second:) 

Type Method

# buildEither(second:)

Provides support for “if-else” statements in multi-statement closures, producing conditional content for the “else” branch.

RealityKitSwiftUIvisionOS 1.0+

``` source
static func buildEither(second: FalseContent) -> ConditionalAttachmentContent where TrueContent : AttachmentContent, FalseContent : AttachmentContent
```

