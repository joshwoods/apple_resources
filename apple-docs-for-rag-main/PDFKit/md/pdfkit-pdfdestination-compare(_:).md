

- PDFKit
- PDFDestination
-  compare(\_:) 

Instance Method

# compare(\_:)

Returns a comparison result that indicates the location of the destination in the document, relative to the current position.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
func compare(_ destination: PDFDestination) -> ComparisonResult
```

## Parameters 

`destination`  

The destination in the document to be located.

## Return Value

A comparison result, indicating the position of the passed-in destination relative to the current position.

## Discussion

If `destination` is between the receiver’s position and the end of the document, `compare` returns `NSOrderedAscending`; if it is between the receiver’s position and the beginning of the document, `compare` returns `NSOrderedDescending`. Otherwise, if `destination` matches the receiver’s position, `compare` returns `NSOrderedSame`.

This method ignores the horizontal component of the destination point (the x value). If the destination’s vertical component (or y value) is PDFDestination, `compare` treats the destination as if its y value is the top point on the destination page.

An exception is raised if `destination` does not have a page associated with it or if its page is associated with a document other than the receiver’s document.

