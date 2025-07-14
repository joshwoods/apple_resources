

- Assignables
- UserIdentityTypeRegistry
-  registerUserIdentityType(typeID:type:) 

Type Method

# registerUserIdentityType(typeID:type:)

Registers a user identity type for use when deserializing the user identity from `Data`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
static func registerUserIdentityType(
    typeID: String,
    type: UI.Type
) where UI : UserIdentity
```

## Parameters 

`typeID`  

A unique type identifier for the user identity to register

`type`  

The type of the user identity to register.

