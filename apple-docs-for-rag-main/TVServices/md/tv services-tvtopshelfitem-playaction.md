

- TV Services
- TVTopShelfItem
-  playAction 

Instance Property

# playAction

The action to perform when the user wants to play the current item.

tvOS 13.0+

``` source
var playAction: TVTopShelfAction? { get set }
```

## Discussion

In a carousel inteface, the first of two buttons invites the user to play the content associated with the current item. The action object you assign to this property provides the title and image to use for that button. When selected, the system loads the action’s URL.

In a sectioned interface, tvOS loads the URL for the specified action when the current item is focused and the user presses the play/pause button.

## See Also

### Assigning Actions to the Item

var displayAction: TVTopShelfAction?

The action to perform when the user wants to see more information for the current item.

