

- Core Graphics
-  CGPDFOperatorTableCreate() 

Function

# CGPDFOperatorTableCreate()

Creates an empty PDF operator table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFOperatorTableCreate() -> CGPDFOperatorTableRef?
```

## Return Value

An empty PDF operator table. In Objective-C, you’re responsible for releasing this object by calling CGPDFOperatorTableRelease(_:).

## Discussion

Call the function CGPDFOperatorTableSetCallback(_:_:_:) to fill the operator table with callbacks.

