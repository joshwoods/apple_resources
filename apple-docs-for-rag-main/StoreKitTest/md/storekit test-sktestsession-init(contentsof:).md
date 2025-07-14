

- StoreKit Test
- SKTestSession
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Initializes the test session with a configuration file you provide through a URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(contentsOf fileURL: URL) throws
```

## Parameters 

`fileURL`  

A file URL for a configuration file with a .`storekit` extension.

## Discussion

The file must have a `.storekit` extension. Create a configuration file in Xcode by selecting File \> New \> File and choosing StoreKit Configuration File.

To return all settings in the test session to the states defined in this StoreKit configuration file, call resetToDefaultState().

## See Also

### Initializing test sessions

convenience init(configurationFileNamed: String) throws

Initializes the test session with the provided configuration file that you include in your application’s bundle.

func resetToDefaultState()

Removes all property overrides and resets all test session settings to their default state.

