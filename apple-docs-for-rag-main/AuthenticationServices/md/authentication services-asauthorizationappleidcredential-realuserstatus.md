

- Authentication Services
- ASAuthorizationAppleIDCredential
-  realUserStatus 

Instance Property

# realUserStatus

A value that indicates whether the user appears to be a real person.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var realUserStatus: ASUserDetectionStatus { get }
```

## Discussion

Use this property’s value as one piece of data when trying to prevent fraud. A value of ASUserDetectionStatus.likelyReal is a hint that the system has a reasonably high confidence that the user is a real person, as opposed to an automated agent, but this isn’t a guarantee.

## See Also

### Detecting User Characteristics

enum ASUserDetectionStatus

Possible values for the real user indicator.

