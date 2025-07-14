

- ARKit
- ARReferenceObject
-  referenceObjects(inGroupNamed:bundle:) 

Type Method

# referenceObjects(inGroupNamed:bundle:)

Loads all reference objects in the specified AR Resource Group in your Xcode project’s asset catalog.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class func referenceObjects(
    inGroupNamed name: String,
    bundle: Bundle?
) -> Set?
```

## Parameters 

`name`  

The name of an AR Resource Group from your Xcode project’s main asset catalog.

`bundle`  

The bundle from which to load asset catalog resources, or `nil` to use your app’s main bundle.

## Return Value

A set of all unique reference objects in the specified group.

## Discussion

To use the objects for detection in a world-tracking AR session, provide this set for your session configuration’s detectionObjects property.

## See Also

### Loading Reference Objects

init(archiveURL: URL) throws

Loads a reference object from the specified file URL.

