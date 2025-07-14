

- RealityKit
- RealityView
-  immersiveEnvironmentPicker(content:) 

Instance Method

# immersiveEnvironmentPicker(content:)

Add menu items to open immersive spaces from a media player’s environment picker.

RealityKitSwiftUIvisionOS 2.0+

``` source
nonisolated
func immersiveEnvironmentPicker(@ViewBuilder content: () -> Content) -> some View where Content : View
```

## Discussion

These items are added alongside recently used system environments.

```
SystemPlayerView(player: player)
    .immersiveEnvironmentPicker {
        Button("Chalet", systemImage: "fireplace") {
            Task {
                await openImmersiveSpace(id: "Chalet")
            }
        }
    }
```

Use a `UIViewControllerRepresentable` instance to display a AVPlayerViewController class in your SwiftUI interface.

```
struct SystemPlayerView: UIViewControllerRepresentable {
    let player: AVPlayer

    func makeUIViewController(context: Context) -> AVPlayerViewController {
        return AVPlayerViewController()
    }

    func updateUIViewController(_ avPlayerViewController: AVPlayerViewController, context: Context) {
        viewController.player = player
    }
}
```

Items will be donated to media players (like AVPlayerViewController) downstream in the hierarchy.

Note

View the sample code in Building an immersive media viewing experience to see an immersive space in action.

