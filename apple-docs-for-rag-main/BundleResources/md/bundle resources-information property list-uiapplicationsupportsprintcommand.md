

- Bundle Resources
- Information Property List
-  UIApplicationSupportsPrintCommand 

Property List Key

# UIApplicationSupportsPrintCommand

A Boolean value that indicates whether the app supports the Command-P keyboard shortcut.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

## Details 

Name  
Supports Print Command

Type  

boolean

## Discussion

When the value for this key is `YES`, the system adds the Command-P keyboard shortcut to the app. When someone enters Command-P while using the app, the system calls the printContent(_:) method on the first responder that implements the method found in the responder chain.

An iPad app running in iPadOS shows a Print command in the discoverability HUD when the value for the UIApplicationSupportsPrintCommand key is `YES`. When the same app runs on a Mac with Apple silicon, the system adds Print and Export to PDF menu commands to the File menu.

When an app built with Mac Catalyst includes the UIApplicationSupportsPrintCommand key with a value of `YES`, the system adds the Print and Export to PDF commands to the File menu. However, the app must also include the com.apple.security.print and com.apple.security.files.user-selected.read-write App Sandbox entitlements to make printing and exporting content available to the app when running in macOS.

## See Also

### External accessories

UISupportedExternalAccessoryProtocols

The protocols that the app uses to communicate with external accessory hardware.

**Name:** Supported external accessory protocols

