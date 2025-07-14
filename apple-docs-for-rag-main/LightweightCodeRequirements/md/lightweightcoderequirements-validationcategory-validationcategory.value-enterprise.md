

- LightweightCodeRequirements
- ValidationCategory
- ValidationCategory.Value
-  enterprise 

Type Property

# enterprise

Indicates that the code is signed by an Apple issued distribution certificate and allowed to run via Provisioning profile.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let enterprise: ValidationCategory.Value
```

## Discussion

This category will match on iOS, watchOS, tvOS, and visionOS apps. On macOS this category will only match on iOS on macOS apps.

