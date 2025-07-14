

- UIKit
- UIStoryboard
-  init(name:bundle:) 

Initializer

# init(name:bundle:)

Creates and returns a storyboard object for the specified resource file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(
    name: String,
    bundle storyboardBundleOrNil: Bundle?
)
```

## Parameters 

`name`  

The name of the storyboard resource file without the filename extension. This method raises an exception if this parameter is `nil`.

`storyboardBundleOrNil`  

The bundle containing the storyboard file and its related resources. If you specify `nil`, this method looks in the main bundle of the current application.

## Return Value

A storyboard object for the specified file. If no storyboard resource file matching `name` exists, an exception is thrown with description: `Could not find a storyboard named 'XXXXXX' in bundle...`.

## Discussion

Use this method to retrieve the storyboard object containing the view controller graph you want to access. All of the resources associated with the storyboard must be in the bundle indicated by the `storyboardBundleOrNil` parameter.

