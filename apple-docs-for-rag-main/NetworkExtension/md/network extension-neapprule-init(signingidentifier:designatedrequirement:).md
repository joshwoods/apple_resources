

- Network Extension
- NEAppRule
-  init(signingIdentifier:designatedRequirement:) 

Initializer

# init(signingIdentifier:designatedRequirement:)

Create an app rule that matches an app with a given signing identifier and a given designated requirement.

macOS 10.11+

``` source
init(
    signingIdentifier: String,
    designatedRequirement: String
)
```

## Parameters 

`signingIdentifier`  

The signing identifier of the app that matches the rule. For apps that are signed using Xcode, the app’s signing identifier is equivalent to the app’s bundle identifier.

`designatedRequirement`  

The designated requirement of the app that matches the rule. The designated requirement for an app can be obtained using the `codesign` command-line developer tool.

## Return Value

A newly-initialized `NEAppRule` object.

## See Also

### Initializing an app rule

init(signingIdentifier: String)

Create an app rule that matches an app with a given signing identifier.

