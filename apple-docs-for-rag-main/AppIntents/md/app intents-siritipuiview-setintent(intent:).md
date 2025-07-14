

- App Intents
- SiriTipUIView
-  setIntent(intent:) 

Instance Method

# setIntent(intent:)

Sets an `AppIntent` for this view. This must be called before presenting the view.

AppIntentsUIKitiOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
final func setIntent(intent: Intent) where Intent : AppIntent
```

## Discussion

The provided `AppIntent` must be a valid App Shortcut for this view to work correctly.

