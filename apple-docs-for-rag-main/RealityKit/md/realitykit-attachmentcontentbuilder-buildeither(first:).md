

- RealityKit
- AttachmentContentBuilder
-  buildEither(first:) 

Type Method

# buildEither(first:)

Provides support for “if” statements in multi-statement closures, producing conditional content for the “then” branch.

RealityKitSwiftUIvisionOS 1.0+

``` source
static func buildEither(first: TrueContent) -> ConditionalAttachmentContent where TrueContent : AttachmentContent, FalseContent : AttachmentContent
```

