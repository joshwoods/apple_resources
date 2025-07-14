

- Core Spotlight
- CSSearchQuery
-  protectionClasses 

Instance Property

# protectionClasses

The protection types of the indexes you want to search.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var protectionClasses: [FileProtectionType] { get set }
```

## Discussion

When creating an index to store your app’s data, you can associate a file protection type with that index to encrypt the data it contains. File protections prevent access to the data unless specific conditions occur. For example, you can make the data available only when the device is unlocked, or make it available after the first successful unlocking of the device. This property indicates which of your app’s protected indexes you want to search.

Possible values for this property are complete, completeUnlessOpen, and completeUntilFirstUserAuthentication. By default, the system retrives the data protection class from the `com.apple.developer.default-data-protection` entitlement, if it exists; otherwise, the default value is completeUntilFirstUserAuthentication.

For more information on how to configure file protection types with an index, see Adding your app’s content to Spotlight indexes.

