

- Bundle Resources
- Information Property List
-  CFBundleExecutable 

Property List Key

# CFBundleExecutable

The name of the bundle’s executable file.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Name  
Executable file

Type  

string

## Discussion

For an app, this key is the executable. For a loadable bundle, it’s the binary that’s loaded dynamically by the bundle. For a framework, it’s the shared library framework and must have the same name as the framework but without the `.framework` extension.

macOS uses this key to locate the bundle’s executable or shared library in cases where the user renames the app or bundle directory.

## See Also

### Launch

NSPrincipalClass

The name of the bundle’s main executable class.

**Name:** Principal class

CLKComplicationPrincipalClass

The name of the class that implements the complication data source protocol.

**Name:** ClockKit Complication - Principal Class

LSEnvironment

Environment variables to set before launching the app.

**Name:** Environment variables

UIApplicationShortcutItems

