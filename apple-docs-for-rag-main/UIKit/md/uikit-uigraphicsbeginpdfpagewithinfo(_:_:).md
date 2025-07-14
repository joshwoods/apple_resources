

- UIKit
-  UIGraphicsBeginPDFPageWithInfo(\_:\_:) 

Function

# UIGraphicsBeginPDFPageWithInfo(\_:\_:)

Marks the beginning of a new page in a PDF context and configures it using the specified custom values.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func UIGraphicsBeginPDFPageWithInfo(
    _ bounds: CGRect,
    _ pageInfo: [AnyHashable : Any]?
)
```

## Parameters 

`bounds`  

A rectangle that specifies the size and location of the new PDF page. This rectangle corresponds to the media box rectangle for the page.

`pageInfo`  

A dictionary that specifies additional page-related information, such as the boxes that define different parts of the page. For a list of keys you can include in this dictionary, see Box Dictionary Keys in doc://com.apple.documentation/documentation/coregraphics/cgpdfcontext. The dictionary is retained by the new page, so you may release it after this function returns.

Specify `nil` if you do not want to associate any additional information with the page.

## Discussion

This function ends any previous page before beginning a new one. It sets the media box of the new page to the value in the kCGPDFContextMediaBox key of the `pageInfo` dictionary, or to the value in the `bounds` parameter if the dictionary does not contain the key.

If the current graphics context is not a PDF context, this function does nothing.

You must call this function or the UIGraphicsBeginPDFPageWithInfo(_:_:) function before you issue any drawing commands.

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

func UIGraphicsGetPDFContextBounds() -> CGRect

Returns the current page bounds.

func UIGraphicsAddPDFContextDestinationAtPoint(String, CGPoint)

Creates a jump destination in the current page.

func UIGraphicsSetPDFContextDestinationForRect(String, CGRect)

Links a rectangular area on the current page to the specified jump destination.

func UIGraphicsSetPDFContextURLForRect(URL, CGRect)

Links a rectangular area on the current page to the specified URL.

