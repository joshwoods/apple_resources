

- Bundle Resources
- Information Property List
-  QLThumbnailMinimumSize 

Property List Key

# QLThumbnailMinimumSize

The minimum size, in points, along one dimension of thumbnails for a Quick Look app’s generator.

iOS 2.0+iPadOS 2.0+macOS 10.0+visionOS 1.0+

## Details 

Name  
Quick Look thumbnail minimum size

Type  

number

## Attributes 

Default: `17.0`

## Discussion

If you set this key, Quick Look uses the GenerateThumbnailForURL property for thumbnail sizes greater than this value. If your app’s generator is fast, you can omit this key so that the thumbnail appears in standard lists.

## See Also

### QuickLook

QLNeedsToBeRunInMainThread

A Boolean value indicating whether a Quick Look app’s generator can be run in threads other than the main thread.

**Name:** Quick Look needs to be run in main thread

QLPreviewHeight

A hint at the height, in points, of a Quick Look app’s previews.

**Name:** Quick Look preview height

QLPreviewWidth

A hint at the width, in points, of a Quick Look app’s previews.

**Name:** Quick Look preview width

QLSupportsConcurrentRequests

A Boolean value indicating whether a Quick Look app’s generator can handle concurrent thumbnail and preview requests.

**Name:** Quick Look supports concurrent requests

