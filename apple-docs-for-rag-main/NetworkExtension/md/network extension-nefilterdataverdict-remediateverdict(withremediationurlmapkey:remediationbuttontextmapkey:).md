

- Network Extension
- NEFilterDataVerdict
-  remediateVerdict(withRemediationURLMapKey:remediationButtonTextMapKey:) 

Type Method

# remediateVerdict(withRemediationURLMapKey:remediationButtonTextMapKey:)

Creates a verdict to drop the current chunk of network data and all subsequent data for the current flow, and provides a remediation URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func remediateVerdict(
    withRemediationURLMapKey remediationURLMapKey: String?,
    remediationButtonTextMapKey: String?
) -> NEFilterDataVerdict
```

## Parameters 

`remediationURLMapKey`  

The key in the Filter Control Provider’s remediationMap dictionary corresponding to the URL of the remediation link to give to the user.

`remediationButtonTextMapKey`  

The key in the Filter Control Provider’s `remediationMap` dictionary that corresponds to the text of the remediation link text to give to the user.

## Return Value

A `NEFilterDataVerdict` object.

## Discussion

When the Filter Data Provider returns this verdict from one of its data filtering methods, the system resolves the verdict as follows:

1.  The system uses the verdict’s `remediationURLMapKey` and `remediationButtonTextMapKey` to look up the remediation URL parameters in the remediationMap dictionary set by the Filter Control Provider.

2.  The system then inserts the remediation URL parameters into the block page and presents it to the user.

The user can tap the URL to appeal the decision to drop the flow. This starts the remediation process, if your app provides one.

## See Also

### Creating data verdicts

class func allow() -> NEFilterDataVerdict

Creates a verdict that tells the system to pass the current chunk of network data and all subsequent data for the current flow to its final destination.

class func drop() -> NEFilterDataVerdict

Creates a verdict that tells the system to drop the current chunk of network data and all subsequent data for the current flow.

class func pause() -> NEFilterDataVerdict

Creates a verdict that tells the system to pause the flow.

class func needRules() -> NEFilterDataVerdict

Creates a verdict that tells the system that the Filter Control Provider needs to update the rules before making a decision about the flow’s data.

init(passBytes: Int, peekBytes: Int)

Creates a verdict that tells the system to pass a chunk of network data to its final destination, and specifies the next chunk of data to provide.

