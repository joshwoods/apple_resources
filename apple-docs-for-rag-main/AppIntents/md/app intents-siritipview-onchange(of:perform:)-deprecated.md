

- App Intents
- SiriTipView
-  onChange(of:perform:) Deprecated

Instance Method

# onChange(of:perform:)

Performs an action when a specified value changes.

AppIntentsSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 7.0–10.0Deprecated

``` source
nonisolated
func onChange(
    of value: V,
    perform action: @escaping (V) -> Void
) -> some View where V : Equatable
```

Deprecated

Use \`onChange\` with a two or zero parameter action closure instead.

## Parameters 

`value`  

The value to check when determining whether to run the closure. The value must conform to the Equatable protocol.

`action`  

A closure to run when the value changes. The closure takes a `newValue` parameter that indicates the updated value.

## Return Value

A view that runs an action when the specified value changes.

## Discussion

Use this modifier to run a closure when a value like an `Environment` value or a `Binding` changes. For example, you can clear a cache when you notice that the view’s scene moves to the background:

```
struct ContentView: View {
    @Environment(\.scenePhase) private var scenePhase
    @StateObject private var cache = DataCache()

    var body: some View {
        MyView()
            .onChange(of: scenePhase) { newScenePhase in
                if newScenePhase == .background {
                    cache.empty()
                }
            }
    }
}
```

SwiftUI passes the new value into the closure. You can also capture the previous value to compare it to the new value. For example, in the following code example, `PlayerView` passes both the old and new values to the model.

```
struct PlayerView: View {
    var episode: Episode
    @State private var playState: PlayState = .paused

    var body: some View {
        VStack {
            Text(episode.title)
            Text(episode.showTitle)
            PlayButton(playState: $playState)
        }
        .onChange(of: playState) { [playState] newState in
            model.playStateDidChange(from: playState, to: newState)
        }
    }
}
```

The system may call the action closure on the main actor, so avoid long-running tasks in the closure. If you need to perform such tasks, detach an asynchronous background task.

Important: This modifier is deprecated and has been replaced with new versions that include either zero or two parameters within the closure, unlike this version that includes one parameter. This deprecated version and the new versions behave differently with respect to how they execute the action closure, specifically when the closure captures other values. Using the deprecated API, the closure is run with captured values that represent the “old” state. With the replacement API, the closure is run with captured values that represent the “new” state, which makes it easier to correctly perform updates that rely on supplementary values (that may or may not have changed) in addition to the changed value that triggered the action.

Important

This modifier is deprecated and has been replaced with new versions that include either zero or two parameters within the closure, unlike this version that includes one parameter. This deprecated version and the new versions behave differently with respect to how they execute the action closure, specifically when the closure captures other values. Using the deprecated API, the closure is run with captured values that represent the “old” state. With the replacement API, the closure is run with captured values that represent the “new” state, which makes it easier to correctly perform updates that rely on supplementary values (that may or may not have changed) in addition to the changed value that triggered the action.

