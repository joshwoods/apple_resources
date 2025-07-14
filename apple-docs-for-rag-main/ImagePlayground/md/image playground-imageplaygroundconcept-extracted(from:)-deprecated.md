

- Image Playground
- ImagePlaygroundConcept
-  extracted(from:) Deprecated

Type Method

# extracted(from:)

Builds a playground concept by extracting multiple concepts from a long text that describes the contents of the image.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
static func extracted(from text: String) -> ImagePlaygroundConcept
```

Deprecated

Use extracted(from text: title:) instead.

## Parameters 

`text`  

Suitable for long strings, like paragraphs or entire documents.

The system will try to extract important or interesting concepts from the string and add them to the playground, so that each concept becomes an input prompt to the diffusion models.

However, if the string does not meet the minimum length required for concept extraction, it might decide to use the string as-is as input prompt.

