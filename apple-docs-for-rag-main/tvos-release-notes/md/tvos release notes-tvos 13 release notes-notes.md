

- tvOS Release Notes
-  tvOS 13 Release Notes 

Article

# tvOS 13 Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

The tvOS 13 SDK provides support for developing tvOS apps for Apple TV devices running tvOS 13. The SDK comes bundled with Xcode 11 available from the Mac App Store. For information on the compatibility requirements for Xcode 11, see Xcode 11 Release Notes.

### AuthenticationServices

#### Known Issues

- Passing both ASAuthorizationAppleIDProvider and ASAuthorizationPasswordProvider to ASAuthorizationController is not currently supported on tvOS. (50897359)

### AVFoundation

#### New Features

- AVFoundation now supports encoding video with alpha channels using HEVC. Videos encoded in this manner are broadly supported in AVFoundation APIs, and by Safari within web pages. Technical details of the format can be found in the Interoperability Profile specification. (8045917)

### MapKit

#### Known Issues

- MKMarkerAnnotationView doesn’t render the default glyph image. (52143655)

  **Workaround:** Set the glyphImage property on MKMarkerAnnotationView instances.

- MKMarkerAnnotationView doesn’t render the markers for annotations using the default tint color. (51908728)

  **Workaround:** Set the markerTintColor property on MKMarkerAnnotationView instances.

### Networking

#### Known Issues

- The urlSession(_:taskIsWaitingForConnectivity:) delegate callback might not function as expected. (54309264)

#### Deprecations

- Removed support for FTP and File URL schemes for Proxy Automatic Configuration (PAC). HTTP and HTTPS are the only supported URL schemes for PAC. This affects all PAC configurations including, but not limited to, configurations set using Settings, System Preferences, Profiles, and URLSession APIs such as connectionProxyDictionary and CFNetworkExecuteProxyAutoConfigurationURL(_:_:_:_:). (28578280)

- The `URLSession` and NSURLConnection APIs no longer support SPDY. Servers should use HTTP 2 or HTTP 1.1. (43391641)

### SwiftUI

#### New Features

- The EnvironmentValues structure has four new properties for reading accessibility values from the environment: accessibilityDifferentiateWithoutColor, accessibilityReduceTransparency, accessibilityReduceMotion, and accessibilityInvertColors. (51712481)

- The `color(_:)` modifier for Text is renamed foregroundColor(_:) for consistency with the more general foregroundColor(_:) view modifier. (50391847)

- The `BindableObject` protocol’s requirement is now `willChange` instead of `didChange`, and should now be sent before the object changes rather than after it changes. This change allows for improved coalescing of change notifications. (51580731)

- The RangeReplaceableCollection protocol is extended to include a remove(atOffsets:) method and the MutableCollection protocol is extended to include a move(fromOffsets:toOffset:) method. Each new method takes IndexSet instances that you use with the doc://com.apple.documentation/documentation/swiftui/foreach/onmove(perform:) and doc://com.apple.documentation/documentation/swiftui/foreach/ondelete(perform:) modifiers on ForEach views. (51991601)

- Added improved presentation modifiers: sheet(isPresented:onDismiss:content:), actionSheet(isPresented:content:), and alert(isPresented:content:) — along with `isPresented` in the environment — replace the existing `presentation(_:)`, `Sheet`, `Modal`, and `PresentationLink` types. (52075730)

- Updated the APIs for creating animations. The basic animations are now named after the curve type — such as linear and easeInOut. The interpolation-based `spring(mass:stiffness:damping:initialVelocity:)` animation is now interpolatingSpring(mass:stiffness:damping:initialVelocity:), and `fluidSpring(stiffness:dampingFraction:blendDuration:timestep:idleThreshold:)` is now spring(response:dampingFraction:blendDuration:) or interactiveSpring(response:dampingFraction:blendDuration:), depending on whether or not the animation is driven interactively. (50280375)

- Added an initializer for creating a Font from a CTFont. (51849885)

#### Known Issues

- Image instances don’t use resizing information configured in asset catalogs. Configure the size of an image using the resizable(capInsets:resizingMode:) modifier instead. (49114577)

#### Deprecations

- The `identified(by:)` method on the Collection protocol is deprecated in favor of dedicated `init(_:id:selection:rowContent:)` and `init(_:id:content:)` initializers. (52976883)

- The `relativeWidth(_:)`, `relativeHeight(_:)`, and `relativeSize(width:height:)` modifiers are deprecated. Use other modifiers like frame(width:height:alignment:) instead. (51494692)

### UIKit

#### Known Issues

- Except for selectionIndicatorTintColor, properties in the new tab bar appearance API aren’t reflected on the screen. (49792597)

### Xcode

#### New Features

- CAMetalLayer is now available in the Simulator. (45101325)

## See Also

### tvOS 13

tvOS 13.4.8 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 13.4.5 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 13.4 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 13.3.1 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 13.3 Release Notes

Update your apps to use new features, and test your apps against API changes.

tvOS 13.2 Release Notes

Update your apps to use new features, and test your apps against API changes.

