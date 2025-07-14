

- Core Graphics
-  CGPDFOperatorTableRetain(\_:) 

Function

# CGPDFOperatorTableRetain(\_:)

Increments the retain count of a CGPDFOperatorTable object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFOperatorTableRetain(_ table: CGPDFOperatorTableRef) -> CGPDFOperatorTableRef
```

## Parameters 

`table`  

A PDF operator table.

## Return Value

The same PDF operator table you passed in as the `table` parameter.

## See Also

### Retaining and Releasing a PDF Operator Table

func CGPDFOperatorTableRelease(CGPDFOperatorTableRef)

Decrements the retain count of a CGPDFOperatorTable object.

