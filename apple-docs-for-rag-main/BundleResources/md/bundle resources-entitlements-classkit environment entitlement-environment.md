

- Bundle Resources
- Entitlements
-  ClassKit Environment Entitlement 

Property List Key

# ClassKit Environment Entitlement

The ClassKit development or production environment for an education app that works with the Schoolwork app.

iOS 11.4+iPadOS 11.4+macOS 11.0+visionOS 1.0+

## Details 

Key  
com.apple.developer.ClassKit-environment

Type  

string

## Possible Values 

`development`  

The environment used to develop and test your app locally, without requiring a Managed Apple ID issued by an educational institution.

`production`  

The environment used by customers of your app who have a Managed Apple ID. This enviroment enables teachers and students to share data through iCloud.

## Discussion

This key specifies the ClassKit environment your app uses to share data with Apple’s Schoolwork app.

To support testing locally, Xcode sets the value to `development` by default. When you upload your app to the App Store, Xcode changes the value to `production`.

To add this entitlement to your app, enable the ClassKit capability in Xcode.

## See Also

### Related Documentation

Enabling ClassKit in your app

Prepare your app and your development environment to adopt ClassKit.

Testing your ClassKit app during development

Use development mode to test your app without a Managed Apple ID.

### Education

com.apple.developer.automatic-assessment-configuration

A Boolean value that indicates whether an app may create an assessment session.

