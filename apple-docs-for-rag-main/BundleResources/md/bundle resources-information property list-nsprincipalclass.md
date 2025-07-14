

- Bundle Resources
- Information Property List
-  NSPrincipalClass 

Property List Key

# NSPrincipalClass

The name of the bundle’s main executable class.

macOS 10.0+

## Details 

Name  
Principal class

Type  

string

## Discussion

The system uses the class identified by this key to set the principalClass property of a bundle when it’s loaded.

Xcode sets the default value of this key to NSApplication for macOS apps, and to UIApplication for iOS and tvOS apps. For other types of bundles, you must set this key in The Info.plist File.

## See Also

### Launch

CLKComplicationPrincipalClass

The name of the class that implements the complication data source protocol.

**Name:** ClockKit Complication - Principal Class

CFBundleExecutable

The name of the bundle’s executable file.

**Name:** Executable file

LSEnvironment

Environment variables to set before launching the app.

**Name:** Environment variables

UIApplicationShortcutItems

