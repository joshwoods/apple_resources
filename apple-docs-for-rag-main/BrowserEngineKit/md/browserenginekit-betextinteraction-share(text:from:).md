

- BrowserEngineKit
- BETextInteraction
-  share(text:from:) 

Instance Method

# share(text:from:)

Presents standard UI for someone to share text from a browser text view.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func share(
    text: String,
    from presentationRect: CGRect
)
```

## Parameters 

`text`  

The text to share.

`presentationRect`  

The area in the view containing the text, which the operating system uses to locate the sharing UI.

## See Also

### Sharing and defining text

func showDictionary(forTextInContext: String, definingTextInRange: NSRange, from: CGRect)

Presents a dictionary definition for the supplied text.

