

- PassKit (Apple Pay and Wallet)
- PKPayLaterView
-  delegate Deprecated

Instance Property

# delegate

A delegate object that receives messages about the changes to the Apple Pay Later view.

iOS 17.0+iPadOS 17.0+visionOS 1.0+

``` source
@MainActor
unowned(unsafe) var delegate: any PKPayLaterViewDelegate { get set }
```

Deprecated

Apple Pay Later is deprecated.

## See Also

### Responding to changes in the view’s height

protocol PKPayLaterViewDelegate

Methods the framework calls when the Apple Pay Later view’s size changes.

Deprecated

