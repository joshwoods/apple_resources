

- App Store Connect API
-  DiagnosticInsightDirection 

Type

# DiagnosticInsightDirection

A string that describes the diagnostic insight direction.

App Store Connect API 3.5+

``` source
string DiagnosticInsightDirection
```

## Possible Values 

`UP`  

`DOWN`  

`UNDEFINED`  

## Possible Values

UP  
The impact of this signature has regressed in the current version compared to previous versions.

DOWN  
The impact of this signature has progressed in the current version compared to previous versions.

UNDEFINED  
No significant change in impact of this signature in the current version compared to previous versions.

## See Also

### Objects

object diagnosticLogs.ProductData.DiagnosticInsights

Information about an insight including a descriptive string, category, and URL.

object diagnosticLogs.ProductData.DiagnosticLogs

The call stack representation and metadata of the diagnostic log.

type DiagnosticInsightType

A string that desribes the diagnostic insight type.

