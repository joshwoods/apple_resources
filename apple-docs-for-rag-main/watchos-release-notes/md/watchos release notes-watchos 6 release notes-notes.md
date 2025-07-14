

- watchOS Release Notes
-  watchOS 6 Release Notes 

Article

# watchOS 6 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The watchOS 6 SDK provides support for developing watchOS apps for Apple Watch devices running watchOS 6. The SDK comes bundled with Xcode 11 beta available from Beta Software Downloads. For information on the compatibility requirements for Xcode 11, see Xcode 11 Release Notes.

Warning

You must update your watch to watchOS 6 beta 2 or later before updating to iOS 13 beta 7 or later, otherwise your watch will no longer be able to connect to your phone. (52854192)

### Networking

#### New Features

- To enhance security, URLSession no longer sniffs the MIME type when the server sends `Content-Type: application/octet-stream`. (7820658)

- NSURLRequest.CachePolicy.reloadRevalidatingCacheData and NSURLRequest.CachePolicy.reloadIgnoringLocalAndRemoteCacheData APIs are now available. (49660334)

- URLSessionWebSocketTask and URLSessionStreamTask are now available for use in watchOS apps. (49779789)

#### Known Issues

- The urlSession(_:taskIsWaitingForConnectivity:) delegate callback might not function as expected. (54309264)

#### Deprecations

- The URLSession and NSURLConnection APIs no longer support SPDY. Servers should use HTTP 2 or HTTP 1.1. (43391641)

### Notifications

#### New Features

- To send a User Notifications push to a watchOS device, a new `apns-push-type` key is now required as part of the APNs request header. Depending on the type of notification, this key can be set to `alert` or `background` and is supported across all Apple platforms. (47099534)

### Podcasts

#### Known Issues

- Asking Siri to play a podcast on Apple Watch might result in an error message. (50392036)

### SwiftUI

#### New Features

- You can now create a Color from a UIColor or NSColor. (49833933)

- NSManagedObject now conforms to ObservableObject. The new `@`FetchRequest property wrapper can drive views from the results of a fetch request, and managedObjectContext is now included in the environment. (50280673)

- Gesture modifiers are renamed for consistency. For example, `tapAction(count:_:)` is renamed onTapGesture(count:perform:), and `longPressAction(minimumDuration:maximumDistance:_:pressing:)` is renamed onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:). (50395282)

- Text now has a default line limit of `nil` so that it wraps by default. (51147116)

- ContentSizeCategory and several other enumerations are now CaseIterable. (51168712)

- `SegmentedControl` is now a style of Picker. (51769046)

- `BindableObject` is replaced by the ObservableObject protocol from the Combine framework. (50800624) You can manually conform to ObservableObject by defining an objectWillChange publisher that emits before the object changes. However, by default, ObservableObject automatically synthesizes objectWillChange and emits before any `@`Published properties change.

  ```
  // RoomStore.swift

  import Foundation

  class RoomStore: ObservableObject {
      @Published var rooms: [Room] = []
  }

  struct Room: Identifiable {
      var id: UUID
      var name: String
      var capacity: Int
      var hasVideo: Bool
  }

  // ContentView.swift
  import SwiftUI

  struct ContentView: View {
      @ObservedObject var store: RoomStore

      var body: some View {
          NavigationView {
              List(store.rooms) { room in
                  RoomCell(room: room)
              }
              .navigationBarTitle("Rooms")
          }
      }
  }
  ```

  ``` @``ObjectBinding ``` is replaced by `@`ObservedObject.

- The EnvironmentValues structure has four new properties for reading accessibility values from the environment: accessibilityDifferentiateWithoutColor, accessibilityReduceTransparency, accessibilityReduceMotion, and accessibilityInvertColors. (51712481)

- The `color(_:)` modifier for Text is renamed foregroundColor(_:) for consistency with the more general foregroundColor(_:) view modifier. (50391847)

- The `BindableObject` protocol’s requirement is now `willChange` instead of `didChange`, and should now be sent before the object changes rather than after it changes. This change allows for improved coalescing of change notifications. (51580731)

- The RangeReplaceableCollection protocol is extended to include a remove(atOffsets:) method and the MutableCollection protocol is extended to include a move(fromOffsets:toOffset:) method. Each new method takes IndexSet instances that you use with the doc://com.apple.documentation/documentation/SwiftUI/ForEach/onmove(perform:) and doc://com.apple.documentation/documentation/SwiftUI/ForEach/ondelete(perform:) modifiers on ForEach views. (51991601)

- Added improved presentation modifiers: sheet(isPresented:onDismiss:content:), actionSheet(isPresented:content:), and alert(isPresented:content:) — along with `isPresented` in the environment — replace the existing `presentation(_:)`, `Sheet`, `Modal`, and `PresentationLink` types. (52075730)

- Updated the APIs for creating animations. The basic animations are now named after the curve type — such as linear and easeInOut. The interpolation-based `spring(mass:stiffness:damping:initialVelocity:)` animation is now interpolatingSpring(mass:stiffness:damping:initialVelocity:), and `fluidSpring(stiffness:dampingFraction:blendDuration:timestep:idleThreshold:)` is now spring(response:dampingFraction:blendDuration:) or interactiveSpring(response:dampingFraction:blendDuration:), depending on whether or not the animation is driven interactively. (50280375)

- Added an initializer for creating a Font from a CTFont. (51849885)

#### Known Issues

- SwiftUI has an API that lets you change the value type of Binding to AnyHashable:

  ```
  let someBinding: Binding = ...
  let typeErasedBinding = Binding(someBinding)
  ```

  Attempting to use this API at compile time results in a linker error on watchOS 6. (53769896)

- A WKInterfaceObjectRepresentable instance with no explicit width might expand to the bounds of its container.

  **Workaround:** Wrap the WKInterfaceObjectRepresentable instance in a GeometryReader to get an explicit width for the view. (53512858)

- Image instances don’t use resizing information configured in asset catalogs. Configure the size of an image using the resizable(capInsets:resizingMode:) modifier instead. (49114577)

#### Deprecations

- SwiftUI APIs deprecated in previous betas are now removed. (52587863, 53310683)

- The `Length` type is replaced by CGFloat. (50654095)

- `TabbedView` is now named TabView. (51012120)

- `HAlignment` and `VAlignment` are now deprecated, use the more flexible HorizontalAlignment or VerticalAlignment types instead and use TextAlignment for text. (51190531)

- The `SelectionManager` protocol is removed, use Optional and Set instances directly for selection. (51557694)

- The `isPresented` environment value is deprecated and replaced with the more general presentationMode value. (51641238)

- The `StaticMember` protocol is deprecated. Use protocol-conforming types directly instead. For example, use an instance of WheelPickerStyle directly rather than the `wheel` static member.(52911961)

- Complex overloads for the background(_:alignment:) and border(_:width:) modifiers are deprecated. Use shapes in a background(_:alignment:) or overlay(_:alignment:) to draw these instead. (53067530)

- The `identified(by:)` method on the Collection protocol is deprecated in favor of dedicated `init(_:id:selection:rowContent:)` and `init(_:id:content:)` initializers. (52976883, 52029393)

  The retroactive conformance of Int to the Identifiable protocol is removed. Change any code that relies on this conformance to pass `\.self` to the `id` parameter of the relevant initializer. Constant ranges of Int continue to be accepted:

  ```
  List(0..

  However, you shouldn’t pass a range that changes at runtime. If you use a variable that changes at runtime to define the range, the list displays views according to the initial range and ignores any subsequent updates to the range.

- Several extensions to the Binding structure are removed. (51624798)

  If you have code such as the following:

  ```
  struct LandmarkList: View {
      var landmark: [Landmark]
      @Binding var favorites: Set

      var body: some View {
          List(landmarks) { landmark in
              Toggle(landmark.name, isOn: self.$favorites.contains(landmarkID))
          }
      }
  }
  ```

  Define the following subscript on the Set structure:

  ```
  extension Set {
      subscript(member: Element) -> Bool {
          get { contains(member) }
          set {
              if newValue {
                  insert(member)
              } else {
                  remove(member)
              }
          }
      }
  }
  ```

  Then, change `self.$favorites.contains(landmarkID)` to `self.$favorites[landmarkID]`.

- The Binding structure’s conditional conformance to the Collection protocol is removed. (51624798)

  If you have code such as the following:

  ```
  struct LandmarkList: View {
      @Binding var landmark: [Landmark]

      var body: some View {
          List(landmarks) { landmark in
              Toggle(landmark.value.name, isOn: landmark[\.isFavorite])
          }
      }
  }
  ```

  Define the following collection type:

  ```
  struct IndexedCollection: RandomAccessCollection {
      typealias Index = Base.Index
      typealias Element = (index: Index, element: Base.Element)

      let base: Base

      var startIndex: Index { base.startIndex }

      var endIndex: Index { base.startIndex }

      func index(after i: Index) -> Index {
          base.index(after: i)
      }

      func index(before i: Index) -> Index {
          base.index(before: i)
      }

      func index(_ i: Index, offsetBy distance: Int) -> Index {
          base.index(i, offsetBy: distance)
      }

      subscript(position: Index) -> Element {
          (index: position, element: base[position])
      }
  }

  extension RandomAccessCollection {
      func indexed() -> IndexedCollection {
          IndexedCollection(base: self)
      }
  }
  ```

  Then, update your code to:

  ```
  struct LandmarkList: View {
      @Binding var landmarks: [Landmark]

      var body: some View {
          List(landmarks.indexed(), id: \.1.id) { (index, landmark) in
              Toggle(landmark.name, isOn: self.$landmarks[index].isFavorite)
          }
      }
  }
  ```

- The `relativeWidth(_:)`, `relativeHeight(_:)`, and `relativeSize(width:height:)` modifiers are deprecated. Use other modifiers like frame(minWidth:idealWidth:maxWidth:minHeight:idealHeight:maxHeight:alignment:) instead. (51494692)

### Xcode

#### Known Issues

- If your watch debugging session continuously times out, you might need to quit and relaunch Xcode after connecting to the internet in order to download the appropriate DeviceSupport files. (50554987)

- The watchOS Mail app and related processes might quit unexpectedly when used within the Simulator. (53799899)

## See Also

### watchOS 6

watchOS 6.2.8 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 6.2.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 6.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 6.1.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 6.1.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

watchOS 6.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

