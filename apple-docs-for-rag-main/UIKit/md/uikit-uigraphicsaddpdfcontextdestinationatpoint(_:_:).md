

- UIKit
-  UIGraphicsAddPDFContextDestinationAtPoint(\_:\_:) 

Function

# UIGraphicsAddPDFContextDestinationAtPoint(\_:\_:)

Creates a jump destination in the current page.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsAddPDFContextDestinationAtPoint(
    _ name: String,
    _ point: CGPoint
)
```

## Parameters 

`name`  

The name of the destination point. The name you assign is local to the PDF document and is what you use when creating links to this destination.

`point`  

A point on the current page of the PDF context.

## Discussion

This function marks the specified point in the current page as the destination of a jump. When the user taps a link that takes them to this jump destination, the PDF document scrolls until the specified point is visible.

If the current graphics context is not a PDF context, this function does nothing.

For information on how to create links to this destination, see the UIGraphicsSetPDFContextDestinationForRect(_:_:) function.

## See Also

### PDF creation

func UIGraphicsBeginPDFContextToData(NSMutableData, CGRect, [AnyHashable : Any]?)

Creates a PDF graphics context that targets the specified mutable data object.

func UIGraphicsBeginPDFContextToFile(String, CGRect, [AnyHashable : Any]?) -> Bool

Creates a PDF graphics context that targets a file at the specified path.

func UIGraphicsEndPDFContext()

Closes a PDF graphics context and pops it from the current context stack.

func UIGraphicsBeginPDFPage()

Marks the beginning of a new page in a PDF context and configures it using default values.

func UIGraphicsBeginPDFPageWithInfo(CGRect, [AnyHashable : Any]?)

Marks the beginning of a new page in a PDF context and configures it using the specified custom values.

func UIGraphicsGetPDFContextBounds() -> CGRect

Returns the current page bounds.

func UIGraphicsSetPDFContextDestinationForRect(String, CGRect)

Links a rectangular area on the current page to the specified jump destination.

func UIGraphicsSetPDFContextURLForRect(URL, CGRect)

Links a rectangular area on the current page to the specified URL.

