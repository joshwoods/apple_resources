

- Network Extension
- NEFilterDataProvider
-  handleRemediation(for:) 

Instance Method

# handleRemediation(for:)

Handle a remediation request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func handleRemediation(for flow: NEFilterFlow) -> NEFilterRemediationVerdict
```

## Parameters 

`flow`  

An NEFilterFlow object containing information about the flow.

## Return Value

An NEFilterRemediationVerdict object indicating how the system should handle the flow of network content.

## Discussion

The system calls this method when the user taps or clicks on the remediation link in the “block” web page in a WebKit browser object and the target of the remediation link is not set to a web page.

`NEFilterDataProvider` subclasses must override this method.

