

- Network Extension
- NEFilterControlProvider
-  handleRemediation(for:completionHandler:) 

Instance Method

# handleRemediation(for:completionHandler:)

Handle a request for remediation from the user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func handleRemediation(
    for flow: NEFilterFlow,
    completionHandler: @escaping (NEFilterControlVerdict) -> Void
)
```

``` source
func handleRemediation(for flow: NEFilterFlow) async -> NEFilterControlVerdict
```

## Parameters 

`flow`  

An NEFilterFlow object containing details about the flow that requires remediation.

`completionHandler`  

A block that must be called when the Filter Control Provider has made a decision about the flow. The NEFilterControlVerdict object passed to this block contains the decision that the Filter Control Provider made about the flow.

## Discussion

This method is called by the system when the Filter Data Provider indicates that the filtering verdict for the given flow is `NEFilterRemediateVerdictNeedRules`. Subclass implementations must override this method and implement whatever steps are necessary to remediate the given flow.

## See Also

### Handling remediation

var remediationMap: [String : [String : NSObject]]?

A dictionary containing sets of strings used to customize the remediation portion of the block page.

let NEFilterProviderRemediationMapRemediationButtonTexts: String

A key in the remediationMap dictionary. The value of this key should be set to a dictionary that maps button text string identifiers to the text to display for the remediation URL link in the block page. The button text string identifiers are defined by the Filter Control Provider app extension.

let NEFilterProviderRemediationMapRemediationURLs: String

A key in the remediationMap dictionary. The value of this key should be set to a dictionary that maps URL identifiers to remediation URLs to be inserted into the block page. The URL identifiers are defined by the Filter Control Provider app extension.

var NEFilterProviderRemediationURLFlowURL: String

This string will be replaced with the full URL of the flow.

var NEFilterProviderRemediationURLFlowURLHostname: String

This string will be replaced with the hostname portion of the flow’s URL.

var NEFilterProviderRemediationURLOrganization: String

This string will be replaced with the value of the organization property set in the filter configuration.

var NEFilterProviderRemediationURLUsername: String

This string will be replaced with the value of the username property set in the filter configuration.

var urlAppendStringMap: [String : String]?

A dictionary containing strings to be appended to URLs.

