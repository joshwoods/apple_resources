

- UIKit
-  UIGraphicsSetPDFContextURLForRect(\_:\_:) 

Function

# UIGraphicsSetPDFContextURLForRect(\_:\_:)

Links a rectangular area on the current page to the specified URL.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsSetPDFContextURLForRect(
    _ url: URL,
    _ rect: CGRect
)
```

## Parameters 

`url`  

The URL to open.

`rect`  

A rectangle on the current page of the PDF context.

## Discussion

You use this function to create external links within a PDF document. If the URL you specify is a type handled by a different application, tapping the rectangle opens that application.

If the current graphics context is not a PDF context, this function does nothing.

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

func UIGraphicsAddPDFContextDestinationAtPoint(String, CGPoint)

Creates a jump destination in the current page.

func UIGraphicsSetPDFContextDestinationForRect(String, CGRect)

Links a rectangular area on the current page to the specified jump destination.

