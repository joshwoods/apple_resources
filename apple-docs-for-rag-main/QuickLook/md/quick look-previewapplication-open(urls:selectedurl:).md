

- Quick Look
- PreviewApplication
-  open(urls:selectedURL:) 

Type Method

# open(urls:selectedURL:)

Previews the provided URLs.

visionOS 2.0+

``` source
final class func open(
    urls: [URL],
    selectedURL: URL? = nil
) -> PreviewSession
```

## Parameters 

`urls`  

An array of URLs to present in the new `PreviewApplication` scene.

`selectedURL`  

If provided and in the array of passed URLs, the URL to select in the presented collection..

## Return Value

A `PreviewSession` instance.

## Discussion

This method launches the preview application with the provided URLs and, optionally, a selected URL.

