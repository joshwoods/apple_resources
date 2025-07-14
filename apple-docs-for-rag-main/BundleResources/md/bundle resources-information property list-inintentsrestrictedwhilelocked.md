

- Bundle Resources
- Information Property List
-  INIntentsRestrictedWhileLocked 

Property List Key

# INIntentsRestrictedWhileLocked

The names of the intent classes your app can’t handle when the user locks the device.

iOS 14.0+iPadOS 14.0+tvOS 14.0+visionOS 1.0+

## Details 

Name  
Restricted While Locked

Type  

array of strings

## Discussion

To specify this information in Xcode, add the intent class name to your app target’s Supported Intents in the Project Editor. Then set the Authentication level to Restricted While Locked.

## See Also

### Intents

INIntentsSupported

The names of the intent classes your app handles directly.

**Name:** Intents eligible for in-app handling

INIntentsRestrictedWhileProtectedDataUnavailable

The names of the intent classes your app can’t handle when the user locks the device or the system blocks access to protected data.

**Name:** Intents restricted while locked or protected data unavailable

INSupportedMediaCategories

Types of media supported by your app’s media-playing intents.

**Name:** Supported intent media categories

