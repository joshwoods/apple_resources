

- Image Playground
- ImagePlaygroundConcept
-  extracted(from:title:) 

Type Method

# extracted(from:title:)

Creates a concept structure from a long-form string and a title that guides the extraction of concepts from that string.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
static func extracted(
    from text: String,
    title: String? = nil
) -> ImagePlaygroundConcept
```

## Parameters 

`text`  

A long text description, such as a paragraph or document. You can specify any length string you want. For strings above a minimum length, the system extracts important or interesting concepts using the contents of `title` as a guide. It converts the concepts it extracts into a separate input prompts for the diffusion model. For strings below the minimum length, the system passes the entire string to the model.

`title`  

A concise summary of the text you pass in the `text` parameter. The system uses this string as a guide to extract concepts from the `text` parameter.

## Return Value

A concept object that encapsulates the concepts from the specified text.

## Discussion

Call this method when you want to use long-form text to generate an image. The method extracts relevant details from the text and uses them to create the returned object.

## See Also

### Describing the image

static func text(String) -> ImagePlaygroundConcept

Creates a concept structure that includes a short text description.

static func drawing(PKDrawing) -> ImagePlaygroundConcept

Creates a concept structure from a PencilKit drawing.

static func image(CGImage) -> ImagePlaygroundConcept

Creates a concept structure from the specified image object.

static func image(URL) -> ImagePlaygroundConcept?

Creates a concept structure from the image at the specified URL.

