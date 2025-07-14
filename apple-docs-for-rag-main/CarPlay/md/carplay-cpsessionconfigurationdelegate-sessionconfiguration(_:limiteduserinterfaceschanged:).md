

- CarPlay
- CPSessionConfigurationDelegate
-  sessionConfiguration(\_:limitedUserInterfacesChanged:) 

Instance Method

# sessionConfiguration(\_:limitedUserInterfacesChanged:)

Tells the delegate that the system changed keyboard or list limits on the user interface.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func sessionConfiguration(
    _ sessionConfiguration: CPSessionConfiguration,
    limitedUserInterfacesChanged limitedUserInterfaces: CPLimitableUserInterface
)
```

## Parameters 

`sessionConfiguration`  

The current session configuration.

`limitedUserInterfaces`  

A bit mask value indicating the user interface limits that changed.

