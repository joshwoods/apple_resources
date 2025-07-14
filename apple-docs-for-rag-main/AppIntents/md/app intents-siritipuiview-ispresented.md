

- App Intents
- SiriTipUIView
-  isPresented 

Instance Property

# isPresented

Determines if the view should be presented to the user.

AppIntentsUIKitiOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor @objc @preconcurrency
dynamic final var isPresented: Bool { get set }
```

## Discussion

Defaults to `true` and gets set to `false` after the dismissal button is tapped. Changing this has no affect if `allowsDismissal` is set to `false`. This value is KVO compliant.

## See Also

### Getting the view’s configuration

var allowsDismissal: Bool

Indicates if the tip view should display a dismissal button

