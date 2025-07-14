

- Core Graphics
-  CGPDFScannerPopNumber(\_:\_:) 

Function

# CGPDFScannerPopNumber(\_:\_:)

Retrieves a real value object from the scanner stack.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFScannerPopNumber(
    _ scanner: CGPDFScannerRef,
    _ value: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`scanner`  

A valid scanner object.

`value`  

On output, points to the real value object popped from the scanner stack.

## Return Value

true if the real value is retrieved successfully; otherwise, false.

## Discussion

The number retrieved from the scanner can be a real value or an integer value. However, the result is always converted to a value of type CGPDFReal.

## See Also

### Getting PDF Objects from the Scanner Stack

func CGPDFScannerPopObject(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFObjectRef?>?) -> Bool

Retrieves an object from the scanner stack.

func CGPDFScannerPopBoolean(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Retrieves a Boolean object from the scanner stack.

func CGPDFScannerPopInteger(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFInteger>?) -> Bool

Retrieves an integer object from the scanner stack.

func CGPDFScannerPopName(CGPDFScannerRef, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>?) -> Bool

Retrieves a character string from the scanner stack.

func CGPDFScannerPopString(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFStringRef?>?) -> Bool

Retrieves a string object from the scanner stack.

func CGPDFScannerPopArray(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Retrieves an array object from the scanner stack.

func CGPDFScannerPopDictionary(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFDictionaryRef?>?) -> Bool

Retrieves a PDF dictionary object from the scanner stack.

func CGPDFScannerPopStream(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFStreamRef?>?) -> Bool

Retrieves a PDF stream object from the scanner stack.

