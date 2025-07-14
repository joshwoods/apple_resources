

- ARKit
- ARReferenceObject
-  init(archiveURL:) 

Initializer

# init(archiveURL:)

Loads a reference object from the specified file URL.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(archiveURL url: URL) throws
```

## Parameters 

`url`  

The local file URL containing the reference object to load.

## Return Value

The reference object contained in the file.

## Discussion

To use the object for detection in a world-tracking AR session, add it to the detectionObjects set in your session configuration.

## See Also

### Loading Reference Objects

class func referenceObjects(inGroupNamed: String, bundle: Bundle?) -> Set&lt;ARReferenceObject>?

Loads all reference objects in the specified AR Resource Group in your Xcode project’s asset catalog.

