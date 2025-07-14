

- AppKit
- NSStoryboard
-  instantiateController(withIdentifier:) 

Instance Method

# instantiateController(withIdentifier:)

Instantiates a specified view controller or window controller from a storyboard.

macOS 10.10+

``` source
func instantiateController(withIdentifier identifier: NSStoryboard.SceneIdentifier) -> Any
```

## Parameters 

`identifier`  

The unique identifier for the controller, which you have specified using the Identity inspector in Interface Builder.

## Return Value

The instantiated view controller or window controller identified by the `identifier` parameter, from the storyboard file. If the specified identifier does not exist (or is `nil`) in the storyboard file, this method raises an exception.

## Discussion

Use this method to create a view controller or window controller object that you want to manipulate and present programmatically. Your controller object must have an identifier string. In Xcode’s storyboard editor, select your controller, display the identity inspector, and place this string in the Storyboard ID field.

This method creates a new instance of the specified controller each time you call it.

## See Also

### Instantiating Storyboard Controllers

func instantiateController&lt;Controller>(identifier: NSStoryboard.SceneIdentifier, creator: ((NSCoder) -> Controller?)?) -> Controller

Creates the specified view controller from the storyboard and initializes it using your custom initialization code.

func instantiateController&lt;Controller>(identifier: NSStoryboard.SceneIdentifier, creator: ((NSCoder) -> Controller?)?) -> Controller

Creates the specified window controller from the storyboard and initializes it using your custom initialization code.

typealias SceneIdentifier

A string that uniquely identifies a view controller or window controller in your storyboard file.

