

- GameKit
- GKDialogController
-  present(\_:) 

Instance Method

# present(\_:)

Presents the dashboard in the window.

macOS 10.8+

``` source
@MainActor
func present(_ viewController: any NSViewController & GKViewController) -> Bool
```

## Parameters 

`viewController`  

A Game Center view controller that represents the dashboard.

## Return Value

true if the dashboard is presented. false if an error occurs.

## Discussion

The dashboard covers the window until the player dismisses it.

## See Also

### Presenting and Dismissing the Dialog

func dismiss(Any)

Dismisses the dashboard.

