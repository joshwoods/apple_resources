

- Core Image
- CIFilter
-  registerName(\_:constructor:classAttributes:) 

Type Method

# registerName(\_:constructor:classAttributes:)

Publishes a custom filter that is not packaged as an image unit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func registerName(
    _ name: String,
    constructor anObject: any CIFilterConstructor,
    classAttributes attributes: [String : Any] = [:]
)
```

## Parameters 

`name`  

A string object that specifies the name of the filter you want to publish.

`anObject`  

A constructor object that implements the `filterWithName` method.

`attributes`  

A dictionary that contains the class display name and filter categories attributes along with the appropriate value for each attributes. That is, the kCIAttributeFilterDisplayName attribute and a string that specifies the display name, and the kCIAttributeFilterCategories and an array that specifies the categories to which the filter belongs (such as kCICategoryStillImage and kCICategoryDistortionEffect). All other attributes for the filter should be returned by the custom `attributes` method implement by the filter.

## Discussion

In most cases you don’t need to use this method because the preferred way to register a custom filter that you write is to package it as an image unit. You do not need to use this method for a filter packaged as an image unit because you register your filter using the `CIPlugInRegistration` protocol. (See Core Image Programming Guide for additional details.)

