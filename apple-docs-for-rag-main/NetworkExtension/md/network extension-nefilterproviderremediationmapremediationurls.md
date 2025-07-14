

- Network Extension
-  NEFilterProviderRemediationMapRemediationURLs 

Global Variable

# NEFilterProviderRemediationMapRemediationURLs

A key in the remediationMap dictionary. The value of this key should be set to a dictionary that maps URL identifiers to remediation URLs to be inserted into the block page. The URL identifiers are defined by the Filter Control Provider app extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
let NEFilterProviderRemediationMapRemediationURLs: String
```

## See Also

### Handling remediation

func handleRemediation(for: NEFilterFlow, completionHandler: (NEFilterControlVerdict) -> Void)

Handle a request for remediation from the user.

var remediationMap: [String : [String : NSObject]]?

A dictionary containing sets of strings used to customize the remediation portion of the block page.

let NEFilterProviderRemediationMapRemediationButtonTexts: String

A key in the remediationMap dictionary. The value of this key should be set to a dictionary that maps button text string identifiers to the text to display for the remediation URL link in the block page. The button text string identifiers are defined by the Filter Control Provider app extension.

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

