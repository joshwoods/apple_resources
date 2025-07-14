

- UIKit
- UIResponder
-  makeTouchBar() 

Instance Method

# makeTouchBar()

Asks the receiving responder to create and configure a Touch Bar object.

Mac Catalyst 13.0+

``` source
@MainActor
func makeTouchBar() -> NSTouchBar?
```

## Return Value

A newly created Touch Bar object.

## Discussion

Override this method in a responder, such as UIViewController, to create and configure a Touch Bar object for the responder.

```
#if targetEnvironment(macCatalyst)
extension RecipeDetailViewController: NSTouchBarDelegate {
    override func makeTouchBar() -> NSTouchBar? {
        let touchBar = NSTouchBar()
        touchBar.delegate = self

        touchBar.defaultItemIdentifiers = [
            .flexibleSpace,
            .deleteRecipe,
            .flexibleSpace,
            .editRecipe,
            .toggleRecipeIsFavorite,
            .flexibleSpace
        ]

        return touchBar
    }

    func touchBar(_ touchBar: NSTouchBar, makeItemForIdentifier identifier: NSTouchBarItem.Identifier) -> NSTouchBarItem? {
        let touchBarItem: NSTouchBarItem?
        // ...
        return touchBarItem
    }

#endif
```

## See Also

### Managing the Touch Bar

var touchBar: NSTouchBar?

The Touch Bar object for the responder.

