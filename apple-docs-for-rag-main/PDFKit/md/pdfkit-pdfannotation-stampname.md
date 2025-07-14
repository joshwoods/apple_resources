

- PDFKit
- PDFAnnotation
-  stampName 

Instance Property

# stampName

The name of the stamp, a text or graphics annotation that emulates a rubber stamp effect.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
var stampName: String? { get set }
```

## Discussion

The default value for this property is `Default`. Additional possible values for `stampName` are: `Approved`, `Asis`, `Confidential`, `Departmental`, `Experimental`, `Expired`, `Final`, `ForComment`, `ForPublicRelease`, `NotApproved`, `NotForPublicRelease`, `Sold`, and `TopSecret`. Custom values are also supported.

