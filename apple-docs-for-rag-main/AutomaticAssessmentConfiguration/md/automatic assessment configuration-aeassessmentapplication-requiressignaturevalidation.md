

- Automatic Assessment Configuration
- AEAssessmentApplication
-  requiresSignatureValidation 

Instance Property

# requiresSignatureValidation

A Boolean that indicates whether the session requires the app to have a valid code signature to run.

Mac Catalyst 15.0+macOS 12.0+

``` source
var requiresSignatureValidation: Bool { get set }
```

## Discussion

When this property is `true`, as it is by default, the system requires that the app’s code signature is valid, and that either Apple distributes the app, or the developer notarizes the app or distributes it through the App Store. You can set the value to `false` to relax these requirements, but do so with caution, because that greatly reduces the security of your assessment session.

