

- AVKit
- AVPlayerView
-  beginTrimming(completionHandler:) 

Instance Method

# beginTrimming(completionHandler:)

Puts the player view into trimming mode.

macOS 10.9+

``` source
@MainActor
func beginTrimming(completionHandler handler: ((AVPlayerViewTrimResult) -> Void)? = nil)
```

``` source
@MainActor
func beginTrimming() async -> AVPlayerViewTrimResult
```

## Parameters 

`handler`  

The callback the system invokes when the user selects the Trim or Cancel button in the trimming UI.

The result passed to the closure indicates whether the user clicked the Trim or Cancel button.

## Mentioned in 

Implementing Trimming in a macOS Player

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func beginTrimming() async -> AVPlayerViewTrimResult
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

An example implementation of the handler block is as follows:

```
@IBAction func beginTrimming(_ sender: AnyObject) {
    playerView.beginTrimming { result in
        if result == .okButton {
            // user selected Trim button (AVPlayerViewTrimResult.okButton)...
        } else {
            // user selected Cancel button (AVPlayerViewTrimResult.cancelButton)...
        }
    }
}
```

This method blocks until the user selects either the Trim or the Cancel button.

## See Also

### Trimming Media

var canBeginTrimming: Bool

A Boolean value that indicates whether the player view can begin trimming.

enum AVPlayerViewTrimResult

Constants that specify an action a user takes when trimming media in a player view.

