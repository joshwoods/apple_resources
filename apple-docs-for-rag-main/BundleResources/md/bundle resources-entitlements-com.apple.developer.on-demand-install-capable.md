

- Bundle Resources
- Entitlements
-  com.apple.developer.on-demand-install-capable 

Property List Key

# com.apple.developer.on-demand-install-capable

A Boolean value that indicates whether a bundle represents an App Clip.

iOS 14.0+iPadOS 14.0+

## Details 

Type  

boolean

## Discussion

Adding an App Clip target to your project as described in Creating an App Clip with Xcode enables a capability called On Demand Install Capable for the App Clip target.

When you code-sign your full app, Xcode embeds the App Clip in the full app and applies the `com.apple.developer.on-demand-install-capable` entitlement. Because of this behavior, the App Clip’s `.entitlements` file doesn’t include this entitlement if you open the file in Xcode’s Project navigator.

To see the entitlement in the `.entitlements` file, first archive the full app, then export the App Clip for distribution as described in Distributing your App Clip. Next, open the Terminal app and run `codesign -d --entitlements :- /path/to/ExampleApp.app/AppClips/ExampleAppClip.app`.

## See Also

### App Clips

Parent Application Identifiers Entitlement

A list of parent application identifiers for an App Clip with exactly one entry.

**Key:** com.apple.developer.parent-application-identifiers

com.apple.developer.associated-appclip-app-identifiers

A list of App Clip identifiers for an app with exactly one entry.

