

- macOS Release Notes
-  macOS Ventura 13.1 Release Notes 

Article

# macOS Ventura 13.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The macOS 13.1 SDK provides support to develop apps for Mac computers running macOS Ventura 13.1. The SDK comes bundled with Xcode 14.2, available from the Mac App Store. For information on the compatibility requirements for Xcode 14.2, see Xcode 14.2 Release Notes.

### Endpoint Security

#### Resolved Issues

- Fixed: Third-party security products using the Endpoint Security API might lose Full Disk Access authorization and stop functioning, even though the product remains visible in System Settings. This issue doesn’t affect authorization granted via MDM. (100857507)

### SwiftUI

#### Deprecations

- In order to improve compiler type-checking performance, we’ve deprecated, and will eventually remove some existing Table initializers. They have been replaced with initializers which require an additional parameter that explicitly specifies the type they generate their contents from. This improves type-check performance by avoiding the need to infer a shared type from the bodies of separate closure parameters. For now, these problematic intiializers have been deprecated.

  The new initializers add the parameter `of:`. The following shows a Table before, and after adoption of the new API:

  ```
  ```

  (101009480)

### SwiftUI Navigation

#### Resolved Issues

- Fixed: NavigationStack on macOS supports animated transitions. Either pass the `path` argument to `NavigationStack` with an animated binding (`$path.binding`), or mutate the path within a `withAnimation` body. The `transition` modifier now has an effect on pushed destinations. For example:

```
private struct AnimatedStacks: View {
    @State private var path: [Int] = []
    private var colors: [Color] = [.red, .green, .blue, .pink]

    var body: some View {
        NavigationStack(path: $path.animation()) {
            VStack {
                List(0..

\(95714581\)

## See Also

### macOS 13

macOS Ventura 13.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Ventura 13.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Ventura 13.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Ventura 13.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

macOS Ventura 13 Release Notes

Update your apps to use new features, and test your apps against API changes.

