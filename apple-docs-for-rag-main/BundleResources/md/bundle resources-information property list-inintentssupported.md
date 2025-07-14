

- Bundle Resources
- Information Property List
-  INIntentsSupported 

Property List Key

# INIntentsSupported

The names of the intent classes your app handles directly.

iOS 14.0+iPadOS 14.0+tvOS 14.0+visionOS 1.0+

## Details 

Name  
Intents eligible for in-app handling

Type  

array of strings

## Discussion

Provide the class name of each INIntent subclass your app can handle. To specify this information in Xcode, add the class names in the Supported Intents section of your app target in the Project Editor.

For more information on handling intents in your app, see application(_:handlerFor:).

Tip

You can start handling an intent in your app even if you want to support the intent in iOS 13. List the intent in the Supported Intents sections for both the app target and the extension target. For an app running on iOS 13, the system routes the intent with handler(for:), and for later iOS versions, it routes the intent with application(_:handlerFor:).

## See Also

### Intents

INIntentsRestrictedWhileLocked

The names of the intent classes your app can’t handle when the user locks the device.

**Name:** Restricted While Locked

INIntentsRestrictedWhileProtectedDataUnavailable

The names of the intent classes your app can’t handle when the user locks the device or the system blocks access to protected data.

**Name:** Intents restricted while locked or protected data unavailable

INSupportedMediaCategories

Types of media supported by your app’s media-playing intents.

**Name:** Supported intent media categories

