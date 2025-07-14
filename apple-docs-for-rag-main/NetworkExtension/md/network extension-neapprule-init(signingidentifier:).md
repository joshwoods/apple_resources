

- Network Extension
- NEAppRule
-  init(signingIdentifier:) 

Initializer

# init(signingIdentifier:)

Create an app rule that matches an app with a given signing identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(signingIdentifier: String)
```

## Parameters 

`signingIdentifier`  

The signing identifier of the app that matches the rule. For apps that are signed using Xcode, the app’s signing identifier is equivalent to the app’s bundle identifier.

## Return Value

A newly-initialized `NEAppRule` object.

## See Also

### Initializing an app rule

init(signingIdentifier: String, designatedRequirement: String)

Create an app rule that matches an app with a given signing identifier and a given designated requirement.

