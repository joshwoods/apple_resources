

- DeviceActivity
- DeviceActivityData
- DeviceActivityData.User
-  nameComponents 

Instance Property

# nameComponents

The user’s name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var nameComponents: PersonNameComponents?
```

## Discussion

You can use this property to construct the user’s name for display. Use the components with an instance of PersonNameComponentsFormatter to create a string representation for the current locale.

