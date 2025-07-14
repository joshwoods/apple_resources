

- Device Management
- ManagedApplicationAttributesResponse
-  ManagedApplicationAttributesResponse.ApplicationAttributesItem 

Device Management Command

# ManagedApplicationAttributesResponse.ApplicationAttributesItem

A dictionary that contains a managed app attributes item.

iOS 7.0+iPadOS 7.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationAttributesResponse.ApplicationAttributesItem
```

## Properties

`Attributes`

ManagedApplicationAttributesResponse.ApplicationAttributesItem.Attributes

The app’s attributes.

`Identifier`

`string`

 (Required) 

The app’s bundle identifier.

Note

For a watchOS app, the identifier is the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired.

## Topics

### Commands

object ManagedApplicationAttributesResponse.ApplicationAttributesItem.Attributes

A dictionary that contains a managed app’s attributes.

## See Also

### Commands

object ManagedApplicationAttributesResponse.ErrorChainItem

A dictionary that describes an error chain item.

