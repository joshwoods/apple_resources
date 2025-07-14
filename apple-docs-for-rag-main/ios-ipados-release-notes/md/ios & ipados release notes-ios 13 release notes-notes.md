

- iOS &amp; iPadOS Release Notes
-  iOS 13 Release Notes 

Article

# iOS 13 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The iOS 13 SDK provides support for developing apps for iPhone devices running iOS 13. The SDK comes bundled with Xcode 11 available from the Mac App Store. For information about Xcode 11, see Xcode 11 Release Notes.

Warning

If your watch is running watchOS 6 beta, you must update it to watchOS 6 beta 2 or later before updating to iOS 13 beta 7 or later, otherwise your watch will no longer be able to connect to your phone. (52854192)

### General

#### Known Issues

- Snapshots for apps that use Metal might have an unexpected appearance in the App Switcher. (53121694)

#### Deprecations

- The UIApplicationExitsOnSuspend key is no longer supported in iOS 13. Update your apps to handle modern multitasking. (43958234)

### Audio

#### New Features

- Voice Processing mode can now be enabled on AVAudioEngine. (50906329)

- New AVAudioNode types can be used to wrap a user-defined block for sending or receiving data in real time.

- A new method is available for an AVAudioEngine-based app to retrieve a list of all nodes attached to an AVAudioEngine instance.

- A new rendering mode in AVAudioEnvironmentNode selects the best spatial audio rendering algorithm automatically based on the output device.

- A new AVAudioSession property allows system sounds and haptics to play while the session actively uses audio input.

- A new enumeration, AVAudioSession.PromptStyle, informs apps which style of voice prompt they should play based on other audio activity in the system.

- AVAudioSession.RouteSharingPolicy now permits apps to specify route-sharing policies so their audio and video routes to the same location as AirPlay.

- Audio Unit Extensions now support user presets that are available across all host applications.

#### Deprecations

- The OpenAL framework is deprecated and remains present for compatibility purposes. Transition to AVAudioEngine for spatial audio functionality.

- AUGraph is deprecated in favor of AVAudioEngine.

- Inter-App audio is deprecated. Use Audio Units for this functionality moving forward.

- Carbon component-based Audio Units are deprecated and support will be removed in a future release.

- Legacy Core Audio HAL audio hardware plug-ins are no longer supported. Use audio server plug-ins for audio drivers moving forward.

### Audio Sharing

#### New Features

- Audio sharing is compatible with AirPods (1st generation or later) and PowerBeats Pro. iPhone 8 or later is required. (51331268)

### AVFoundation

#### New Features

- AVFoundation now supports encoding video with alpha channels using HEVC. Videos encoded in this manner are broadly supported in AVFoundation APIs, and by Safari within web pages. Technical details of the format can be found in the Interoperability Profile specification. (8045917)

### Core Haptics

#### Known Issues

- By default, haptics are disabled when microphone recording begins. You can override this by setting the AVAudioSession property allowHapticsAndSystemSoundsDuringRecording to `true` before activating its audio session. (25811898)

- Events — such as audioContinuous, hapticContinuous, and audioCustom — can’t be resumed during the event; no output occurs for that event, only for subsequent events. This applies to playback at a specific time offset, seeking, and resuming.(29274583)

- CHHapticDynamicParameter instances with nonzero relative times that are sent as part of a sendParameters(_:atTime:) call on a CHHapticAdvancedPatternPlayer with the `atTime` parameter set to `0.0` are incorrectly applied at the beginning of the CHHapticPattern, instead of the expected nonzero relative time. This doesn’t occur on a CHHapticPatternPlayer. (46316890)

- Both vibrations generated through AudioServicesPlaySystemSound(_:) and vibration patterns generated through the user-created tap-to-vibrate UI are attenuated when compared to prior versions of iOS. (47448156)

- Parameter Curves are not supported with a CHHapticAdvancedPatternPlayer, only a CHHapticPatternPlayer. No error is generated when a CHHapticPattern containing a Parameter Curve is passed to a CHHapticAdvancedPatternPlayer. (47891515)

- Brief audio distortion occurs when starting a Playback category app such as Music in the background. For example, brief distortion occurs if you start the app from Control Center while Core Haptics audio playback using a playAndRecord audio session is already underway. (48121467)

- Following any decompression to uncompressed floating-point samples, the total limit on all audioCustom resources per process is eight megabytes. (48659023)

- Multiple overlapping Parameter Curves for the same CHHapticDynamicParameter.ID might result in playback artifacts. (50026384)

- The maximum duration for a hapticContinuous haptic event is 30 seconds. Events exceeding this limit can be constructed and accepted by CHHapticPatternPlayer, but haptic playback will fade out after 30 seconds. (51322525)

### Core Image

#### New Features

- The init(imageURL:options:) and init(imageData:options:) initializers no longer support RAW version 5 and earlier. Version 6 and later remain supported. (50911303)

- Added new APIs for instantiating and modifying the built-in Core Image filters.

- The CICoreMLModel filter is enhanced to support models with an input or output of type MLFeatureType.multiArray.

- Metal CIKernel instances support arguments with arbitrarily structured data.

- Metal CIKernel instances support returning a group of 2 × 2 pixels.

- The integer values of CIFormat symbols, such as ARGB8, have changed to a new set of values that are consistent across platforms. The former values remain supported for backward compatibility; however, you should avoid dependancies on specific numerical values.

### Find My

#### Known Issues

- When performing an action in Find My that generates an email, you might see references to the Find My Friends and Find My iPhone apps. (51123613)

### Health

#### Known Issues

- Health and Activity features will stop working if you set your Period Length to be longer than your Cycle Length in Cycle Tracking options. Ensure your Period Length is set to a shorter duration than your Cycle Length. (54313089)

### iCloud

#### Known Issues

- After updating to iOS 13 beta 6 or later, iCloud Drive might synchronize for an extended period of time. If you notice any missing files, they can be found in a Recovered Files folder under On My iPhone within the Files app. (53772753)

- When creating a new Pages, Numbers, or Keynote document in a shared folder, you might see the message: “Couldn’t connect to iCloud.” (50827963)

  **Workaround:** Close and reopen the document.

### Mail

#### New Features

- Ignore Blocked Senders can now be enabled in Settings \> Mail. The blocked contacts list is shared with Messages, FaceTime, and Phone. (50775961)

### Media Player

#### Known Issues

- Playback stops if an app using MediaPlayerFramework to play catalog content is backgrounded. (54131440)

### Metal

#### Known Issues

- The sparse texture API cannot be used from Swift in iOS 13. The issue is resolved in iOS 13.1 beta. (54146130)

- In iOS 13, if you refer to a sparse texture in an argument buffer you must explicitly call useResource(_:usage:stages:) on the texture rather than calling useHeap(_:) on the heap. (54605833)

### Music

#### Known Issues

- The state of the Sync Library switch in Settings \> Music might inaccurately reflect the current state of the feature on your device. If you don’t want the feature enabled, ensure the switch is off. If your music library doesn’t appear to be in sync with other devices, try toggling the switch off then on again. (53957863)

### Networking

#### New Features

- To enhance security, URLSession no longer sniffs the MIME type when the server sends `Content-Type: application/octet-stream`. (7820658)

- NSURLRequest.CachePolicy.reloadRevalidatingCacheData and NSURLRequest.CachePolicy.reloadIgnoringLocalAndRemoteCacheData APIs are now available. (49660334)

- Starting with iOS 13 beta 4, the copy attribute of the httpBodyStream property of NSMutableURLRequest is enforced. If the body data is mutated after the property setter has been called, data sent in the HTTP request won’t include that mutation. Invoking the property getter no longer returns a NSMutableData reference, even when the setter was invoked with data of that type. As of iOS 13 beta 5, apps built using the iOS 12 SDK or previous SDKs use the legacy behavior. (53427882)

- The CNCopyCurrentNetworkInfo API has changed to address privacy. Please refer to the updated API documentation and headers for more details. (52707167)

- All URLSessionTask instances with a `GET` HTTP method that contain a body now produce the error NSURLErrorDataLengthExceedsMaximum. (46025234)

#### Known Issues

- The urlSession(_:taskIsWaitingForConnectivity:) delegate callback might not function as expected. (54309264)

#### Deprecations

- Removed support for FTP and File URL schemes for Proxy Automatic Configuration (PAC). HTTP and HTTPS are the only supported URL schemes for PAC. This affects all PAC configurations including, but not limited to, configurations set using Settings, System Preferences, Profiles, and URLSession APIs such as connectionProxyDictionary and CFNetworkExecuteProxyAutoConfigurationURL(_:_:_:_:). (28578280)

- The URLSession and NSURLConnection APIs no longer support SPDY. Servers should use HTTP 2 or HTTP 1.1. (43391641)

### Notes

#### Known Issues

- Using search in Notes might produce unexpected results. (48238242)

- If you select colored drawing strokes with the lasso tool and then rotate your device to landscape mode, the strokes will revert to black. (54246012)

### PencilKit

#### Known Issues

- If your app links PencilKit, please refrain from attempting to submit it to the App Store until further notice. (53811027)

### RealityKit

#### Known Issues

- Reality Files with object anchors don’t anchor to those objects in AR Quick Look or in applications. (53689364)

- The camera feed will remain visible at the base of objects loaded from a Reality File when ARView.Environment.Background is set to `ARView.Environment.Background.skybox(_:)` (53715030)

  **Workaround**: Turn off grounding shadows when setting the background to `ARView.Environment.Background.skybox(_:)` by setting ARView.RenderOptions to disableGroundingShadows.

### Screen Time

#### Known Issues

- If you enable Share Across Devices, Screen Time settings don’t sync with iCloud until your iOS device is restarted. Any edits you make to your Screen Time settings on that device before restarting are lost. (50194586)

### Siri

#### Known Issues

- Shortcuts automations are temporarily unavailable. (53182885)

- The supportsOnDeviceRecognition property always returns `false` the first time it’s accessed. After a few seconds, accessing it again returns the correct value. (47822242)

- Shortcuts opened on iOS 13 are automatically upgraded and can no longer be opened on iOS 12. If a device with iOS 12 and a device with iOS 13 share an iCloud account, shortcuts might become unusable on the device running iOS 12. (50873839)

  **Workaround:** Disable iCloud Sync between devices running iOS 13 and devices running iOS 12.

- Currently, the only supported response for doc://com.apple.documentation/documentation/SiriKit/INSearchForMediaIntent is doc://com.apple.documentation/documentation/SiriKit/INSearchForMediaIntentResponseCode/continueInApp. (51010311)

### SwiftUI

#### New Features

- You can now create a Color from a UIColor or NSColor. (49833933)

- NSManagedObject now conforms to ObservableObject. The new `@`FetchRequest property wrapper can drive views from the results of a fetch request, and managedObjectContext is now included in the environment. (50280673)

- Gesture modifiers are renamed for consistency. For example, `tapAction(count:_:)` is renamed onTapGesture(count:perform:), and `longPressAction(minimumDuration:maximumDistance:_:pressing:)` is renamed onLongPressGesture(minimumDuration:maximumDistance:pressing:perform:). (50395282)

- Text now has a default line limit of `nil` so that it wraps by default. (51147116)

- ContentSizeCategory and several other enumerations are now CaseIterable. (51168712)

- `SegmentedControl` is now a style of Picker. (51769046)

- `BindableObject` is replaced by the ObservableObject protocol from the Combine framework. (50800624)

  You can manually conform to ObservableObject by defining an objectWillChange publisher that emits before the object changes. However, by default, ObservableObject automatically synthesizes objectWillChange and emits before any `@`Published properties change.

  ```
  // RoomStore.Swift

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

  // ContentView.Swift
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

  `@ObjectBinding` is replaced by `@`ObservedObject.

- The Identifiable protocol is now part of the Swift standard library. As a result, your model files no longer need to import the SwiftUI framework. (SE-0261)

- The EnvironmentValues structure has four new properties for reading accessibility values from the environment: accessibilityDifferentiateWithoutColor, accessibilityReduceTransparency, accessibilityReduceMotion, and accessibilityInvertColors. (51712481)

- The `color(_:)` modifier for Text is renamed foregroundColor(_:) for consistency with the more general foregroundColor(_:) view modifier. (50391847)

- The `BindableObject` protocol’s requirement is now `willChange` instead of `didChange`, and should now be sent before the object changes rather than after it changes. This change allows for improved coalescing of change notifications. (51580731)

- The RangeReplaceableCollection protocol is extended to include a remove(atOffsets:) method and the MutableCollection protocol is extended to include a move(fromOffsets:toOffset:) method. Each new method takes IndexSet instances that you use with the doc://com.apple.documentation/documentation/SwiftUI/ForEach/onmove(perform:) and doc://com.apple.documentation/documentation/SwiftUI/ForEach/ondelete(perform:) modifiers on ForEach views. (51991601)

- Added improved presentation modifiers: sheet(isPresented:onDismiss:content:), actionSheet(isPresented:content:), and alert(isPresented:content:) — along with `isPresented` in the environment — replace the existing `presentation(_:)`, `Sheet`, `Modal`, and `PresentationLink` types. (52075730)

- Updated the APIs for creating animations. The basic animations are now named after the curve type — such as linear and easeInOut. The interpolation-based `spring(mass:stiffness:damping:initialVelocity:)` animation is now interpolatingSpring(mass:stiffness:damping:initialVelocity:), and `fluidSpring(stiffness:dampingFraction:blendDuration:timestep:idleThreshold:)` is now spring(response:dampingFraction:blendDuration:) or interactiveSpring(response:dampingFraction:blendDuration:), depending on whether or not the animation is driven interactively. (50280375)

- Added an initializer for creating a Font from a CTFont. (51849885)

- You can style a NavigationView using two new style properties: StackNavigationViewStyle and DoubleColumnNavigationViewStyle. By default, navigation views on iPhone and Apple TV visually reflect a navigation stack, while on iPad and Mac, a split-view styled navigation view displays. (51636729)

  When using the DoubleColumnNavigationViewStyle style, you can provide two views when creating a navigation view — the first is the primary and the second is the detail. For example:

  ```
  NavigationView {
      MyPrimaryView()
      MyDetailView()
  }
  .navigationViewStyle(DoubleColumnNavigationViewStyle())
  ```

#### Known Issues

- Image instances don’t use resizing information configured in asset catalogs. Configure the size of an image using the resizable(capInsets:resizingMode:) modifier instead. (49114577)

- Apps containing SwiftUI inside a Swift package might not run on versions of iOS earlier than iOS 13. (53706729)

  **Workaround**: When back-deploying to an OS which doesn’t contain the SwiftUI framework, add the `-weak_framework SwiftUI` flag to the Other Linker Flags setting in the Build Settings tab. See Frameworks and Weak Linking for more information on weak linking a framework. This workaround doesn’t apply when using dynamically linked Swift packages which import SwiftUI.

#### Deprecations

- SwiftUI APIs deprecated in previous betas are now removed. (52587863, 53310683)

- `NavigationDestinationLink` and `DynamicNavigationDestinationLink` are deprecated; their functionality is now included in NavigationLink. (50630794)

- The `Length` type is replaced by CGFloat. (50654095)

- `TabbedView` is now named TabView. (51012120)

- `HAlignment` and `VAlignment` are now deprecated, use the more flexible HorizontalAlignment or VerticalAlignment types instead and use TextAlignment for text. (51190531)

- The `SelectionManager` protocol is removed, use Optional and Set instances directly for selection. (51557694)

- The `isPresented` environment value is deprecated and replaced with the more general presentationMode value. (51641238)

- The `StaticMember` protocol is deprecated. Use protocol-conforming types directly instead. For example, use an instance of WheelPickerStyle directly rather than the `wheel` static member.(52911961)

- Complex overloads for the background(_:alignment:) and border(_:width:) modifiers are deprecated. Use shapes in a background(_:alignment:) or overlay(_:alignment:) to draw these instead. (53067530)

- The `identified(by:)` method on the Collection protocol is deprecated in favor of dedicated init(_:id:rowContent:) and init(_:id:content:) initializers. (52976883, 52029393)

  The retroactive conformance of Int to the Identifiable protocol is removed. Change any code that relies on this conformance to pass `\.self` to the `id` parameter of the relevant initializer. Constant ranges of `Int` continue to be accepted:

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

### Third-Party Apps

#### Known Issues

- You might be unable to stream to a Chromecast device. (51334673)

### UIKit

#### New Features

- The UITableViewCell class no longer changes the backgroundColor or isOpaque properties of the contentView and any of its subviews when cells become highlighted or selected. If you are setting an opaque `backgroundColor` on any subviews of the cell inside (and including) the `contentView`, the appearance when the cell becomes highlighted or selected might be affected. The simplest way to resolve any issues with your subviews is to ensure their `backgroundColor` is set to `nil` or clear, and their `opaque` property is `false`. However, if needed you can override the setHighlighted(_:animated:) and setSelected(_:animated:) methods to manually change these properties on your subviews when moving to or from the highlighted and selected states. (13955336)

- Since iOS 8, using UISearchController with UINavigationController has required setting the definesPresentationContext property of the top view controller to `true`. Failure to do so leads to subtle bugs that can be hard to detect and debug. Starting in iOS & iPadOS 13 beta, if a view controller’s navigationItem has a non-`nil` searchController, when the view controller is shown in a navigation controller, UINavigationController automatically sets that view controller’s definesPresentationContext property to `true`. If you are targeting earlier versions of iOS, set this property before your search controller becomes active. (31338934)

- The UIRefreshControl class no longer directly modifies the contentInset of its scroll view. Instead, its adjustments to the content inset will be incorporated into the scroll view’s adjustedContentInset. The only exception is when the scroll view’s contentInsetAdjustmentBehavior is set to UIScrollView.ContentInsetAdjustmentBehavior.never, in which case the UIRefreshControl instance will modify the `contentInset` directly as it did in previous releases. (35866834)

- If you implement self-sizing cells in a UITableView by overriding sizeThatFits(_:) without using Auto Layout, the height you return is interpreted as the desired height for the `contentView` of the cell, and UITableViewCell automatically adds any additional height needed to allow room for the cell separator. If you implement manual self-sizing this way, the cell’s `contentView` width is guaranteed to be accurate for you to use in manual layout calculations when sizeThatFits(_:) is called on the UITableViewCell. (39742612)

- Trait environments, such as views and view controllers, now have their `traitCollection` property populated with traits during initialization. These initial traits represent a prediction of the ultimate traits that the trait environment will receive when it gets added to the hierarchy. Because the traits that are populated during initialization are just a prediction, they might differ from the traits that are received once actually in the hierarchy. Therefore, when possible you should wait to perform work that uses the `traitCollection` until the view, or view controller’s view, has moved into the hierarchy — meaning window returns a non-`nil` value — so that you don’t have to throw away any work done using the predicted traits if the actual traits are different. The best time to use the `traitCollection` is during layout, such as inside layoutSubviews(), viewWillLayoutSubviews(), or viewDidLayoutSubviews().

- The traitCollectionDidChange(_:) method is only called when the value of a trait changes. Importantly, because the trait collection is now initialized to a prediction of the ultimate traits in the destination hierarchy, when the initial predicted traits match the ultimate traits in the hierarchy, traitCollectionDidChange(_:) will not be called when the trait environment is added to the hierarchy. Because traitCollectionDidChange(_:) is intended to be an invalidation callback to notify you that one or more traits changed, audit your existing implementations of this method, as well as the UIContentContainer method willTransition(to:with:), for places where you might have been relying on it to trigger initial setup. The best place to lazily perform work that uses the `traitCollection` is inside one of the `layoutSubviews` methods discussed above, but remember that these layout methods are called any time layout occurs so be sure to avoid repeating work when you don’t need to. (46818941)

- You can now enable debug logging to easily see when traitCollectionDidChange(_:) or willTransition(to:with:) is called on your own classes. Turn on the logging by using the following launch argument: `-UITraitCollectionChangeLoggingEnabled YES`. You might want to temporarily disable the Main Thread Checker while using this launch argument and running your app from Xcode to avoid extra log messages for unrelated classes. (47858564)

- The UITableViewCell class’s contentView property is always laid out edge-to-edge with adjacent accessories, both on the leading and the trailing side. This streamlines the layout code so developers who want the correct default offset no longer have to align their content with the content view border or the layout margin depending on whether there is an accessory on the trailing side or not. You should now always lay out their code on the layout margins of the cell’s content view to get the default system insets. These insets will be adjusted automatically based on the accessories visible in the cell to match the system’s default spacing. (48214114)

- You can now invoke a custom initializer from a creation block that’s passed through instantiateInitialViewController(creator:) or instantiateViewController(identifier:creator:). This makes it possible for you to initialize view controllers with additional context and arguments, while taking advantage of defining them in a storyboard through Interface Builder. A custom controller initializer must call its `super.init(coder:)` method and pass the coder argument that it receives through the creation block. (48313869)

#### Known Issues

- Specifying `UIWindowScene.DestructionRequestOptions` in Swift is currently unavailable. (51036709)

### Watch

#### Known Issues

- Complications might disappear from Apple Watch after updating to iOS 13 if your watch isn’t running watchOS 6. (50507942)

### Xcode

#### New Features

- CAMetalLayer is now available in Simulator. (45101325)

#### Known Issues

- Donated shortcuts might not appear in Search while using the simulator. (50832782)

  **Workaround:** Test on a device with Settings \> Developer \> Display Recent Shortcuts enabled.

- Changing the volume level in Simulator while a video is playing in Safari mutes the audio. (51207286)

## See Also

### iOS &amp; iPadOS 13

iOS & iPadOS 13.7 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.6 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.3.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

iOS & iPadOS 13.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

