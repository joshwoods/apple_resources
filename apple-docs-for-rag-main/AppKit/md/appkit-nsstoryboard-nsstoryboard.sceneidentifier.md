

- AppKit
- NSStoryboard
-  NSStoryboard.SceneIdentifier 

Type Alias

# NSStoryboard.SceneIdentifier

A string that uniquely identifies a view controller or window controller in your storyboard file.

macOS

``` source
typealias SceneIdentifier = String
```

## Discussion

Set scene identifiers in your storyboard by assigning a value to the Storyboard ID attribute.

## See Also

### Instantiating Storyboard Controllers

func instantiateController(withIdentifier: NSStoryboard.SceneIdentifier) -> Any

Instantiates a specified view controller or window controller from a storyboard.

func instantiateController&lt;Controller>(identifier: NSStoryboard.SceneIdentifier, creator: ((NSCoder) -> Controller?)?) -> Controller

Creates the specified view controller from the storyboard and initializes it using your custom initialization code.

func instantiateController&lt;Controller>(identifier: NSStoryboard.SceneIdentifier, creator: ((NSCoder) -> Controller?)?) -> Controller

Creates the specified window controller from the storyboard and initializes it using your custom initialization code.

