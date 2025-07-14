

- MapKit
-  MKMapView 

Class

# MKMapView

An embeddable map interface, similar to the one that the Maps app provides.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
class MKMapView
```

## Overview

Use this class as-is to display map information and to manipulate the map contents from your app. The map view supports several display styles, including the MKStandardMapConfiguration that provides rich 2D and 3D presentations, an MKHybridMapConfiguration that provides a hybrid satellite map presentation, and MKImageryMapConfiguration that provides an imagery-based map presentation. Each of these map configurations support customization properties that refine specific elements of the map’s presentation.

You can center the map on specific coordinates, specify the size of the area you want to display, and annotate the map with custom information. When you initialize a map view, you specify the initial region for that map to display by setting the region property of the map. MapKit defines a region by a center point and a horizontal and vertical distance, referred to as the *span*. The *span* defines how much of the map is visible, and is also how you set the zoom level. For example, specifying a large span results in the user seeing a wide geographical area at a low zoom level, whereas specifying a small span results in a more narrow geographical area and a higher zoom level.

In addition to setting the span programmatically, the `MKMapView` class supports many standard interactions for changing the position and zoom level of the map. In particular, map views support flick and pinch gestures for scrolling around the map and zooming in and out. The map view enables support for these gestures by default. You can enable and disable them using the isScrollEnabled and isZoomEnabled properties.

You can also use projected map coordinates instead of regions to specify some values. When you project the curved surface of the globe onto a flat surface, you get a two-dimensional version of a map where longitude lines appear to be parallel. To specify locations and distances, you use the MKMapPoint, MKMapSize, and MKMapRect data types.

Don’t subclass the `MKMapView` class itself. You can get information about the map view’s behavior by providing a delegate object. The map view calls the methods of your custom delegate to let it know about changes in the map status and to coordinate the display of custom annotations. The delegate object can be any object in your app as long as it conforms to the MKMapViewDelegate protocol. For more information about implementing the delegate object, see MKMapViewDelegate.

In macOS 10.14 and later, you can apply a light or dark appearance to your maps by modifying the appearance property of your map view (or one of its ancestor views). Even if you specify a custom appearance, users can use the Maps app to force all maps to adopt a light appearance. Use the map view’s effectiveAppearance property to determine the actual appearance of your map. For information about how to set view appearances, see Choosing a Specific Appearance for Your macOS App.

### Annotating the map

The `MKMapView` class supports the ability to annotate the map with custom information. Because a map may have large numbers of annotations, map views differentiate between the annotation objects MapKit uses to manage the annotation data and the view objects for presenting that data on the map.

An *annotation object* is any object that conforms to the MKAnnotation protocol. Typically, you implement annotation objects using existing classes in your app’s data model. This allows you to manipulate the annotation data directly, but still make it available to the map view. Each annotation object contains information about the annotation’s location on the map, along with descriptive information that the map can display in a callout.

An *annotation view*,\_ \_which is an instance of the MKAnnotationView class, handles the presentation of annotation objects on the screen. An annotation view is responsible for presenting the annotation data in a way that makes sense. For example, the Maps app uses a marker icon to denote specific points of interest on a map. The MapKit framework offers the MKMarkerAnnotationView class for similar annotations in your own apps. You can also create annotation views that cover larger portions of the map.

Because the map view needs annotation views only when they’re onscreen, the `MKMapView` class provides a mechanism for queueing annotation views that aren’t in use. The map view detaches annotation views with a reuse identifier and queues them internally when they move offscreen. This feature improves memory use by keeping only a small number of annotation views in memory at once, and by recycling the views you do have. It also improves scrolling performance by alleviating the need to create new views while the map is scrolling.

When configuring your map interface, be sure to add all of your annotation objects right away. The map view uses the coordinate data in each annotation object to determine when the corresponding annotation view needs to appear onscreen. When an annotation moves onscreen, the map view asks its delegate to create a corresponding annotation view. If your app has different types of annotations, it can define different annotation view classes to represent each type.

### Adding overlays to the map

You can use overlays to layer content over a wide portion of the map. An *overlay* object is any object that conforms to the MKOverlay protocol. An overlay object is a data object that contains the points that specify the shape and size of the overlay and its location on the map. Overlays can represent shapes like circles, rectangles, multisegment lines, and simple or complex polygons. You can also define your own custom overlays to represent other shapes.

*Overlay renderer* objects, which are instances of the MKOverlayRenderer class, handle the presentation of an overlay. The job of the renderer is to draw the overlay’s content onto the screen when the map view requests it. For example, if you have a simple overlay that represents a bus route, you can use a polyline renderer to draw the line segments that trace the route of the bus. You can also define a custom renderer that draws both the bus route and icons at the location of each bus stop. When specifying overlays, you can add them to specific levels of the map, which tells the map view to render them above or below other types of map content.

When configuring your map interface, you can add overlay objects at any time. The map view uses the data in each overlay object to determine when the corresponding overlay view needs to appear onscreen. When an overlay moves onscreen, the map view asks its delegate to create a corresponding overlay renderer.

### Adding points of interest to the map

In iOS16 and macOS 13, and later, you can configure the map view to allow people to interact with a wide variety of points of interest (POIs) the map displays. These are instances of the MKMapFeatureAnnotation class, and cover a wide variety of elements visible on the map, including:

- Points of interest, such as museums, cafes, parks, and schools.

- Territorial boundaries, such as national borders, state boundaries, and neighborhoods.

- Features on the Earth’s surface, such as mountain ranges, rivers, and ocean basins.

You can control which features a person can interact with by configuring one of the MKMapConfiguration subclasses that defines the map’s presentation. Create an `MKMapConfiguration` with a set of MKMapFeatureOptions that describe the categories of POIs the map responds to. To further refine the specific kinds of points of interest the map display presents, use an MKPointOfInterestFilter.

When a person interacts with a specific POI, the framework calls your delegate object with one of the MKMapViewDelegate protocol methods, depending on whether the person selects or deselects a specific POI. These methods give your app a chance to respond to the selection or deselection of an element. Depending on the kind of element, you can decide whether you want to customize the display characteristics in the case of a POI, or in the case of territories or geographic map features, you can create custom interactions to display information.

### Adding Look Around views to the map

iOS16 and macOS 13, and later, support the inclusion of a Look Around view within the map view. Look Around allows people to explore the environment at street level. You request a Look Around view by creating an MKLookAroundSceneRequest with either an MKMapItem or a CLLocationCoordinate2D, and if there’s Look Around imagery available for the specified location, the framework returns an MKLookAroundScene for you to display using an MKLookAroundViewController.

## Topics

### Configuring the map appearance

var preferredConfiguration: MKMapConfiguration

The characteristics of the map view, including the map type and features the map displays.

var pitchButtonVisibility: MKFeatureVisibility

A value that indicates whether the map’s pitch button is visible.

var showsUserTrackingButton: Bool

A Boolean value that indicates whether the map displays the user tracking button.

class MKMapConfiguration

An abstract class that represents the shared elements of map configurations.

class MKStandardMapConfiguration

The class that represents the default map presentation, which is a street map that shows the position of all roads and some road names.

class MKHybridMapConfiguration

The class that represents a satellite image of the area with road and road name information layers on top.

class MKImageryMapConfiguration

The class that represents an imagery-based map presentation, such as one using satellite imagery.

### Customizing the map view behavior

var delegate: (any MKMapViewDelegate)?

The receiver’s delegate.

protocol MKMapViewDelegate

Optional methods that you use to receive map-related update messages.

### Accessing map properties

enum MKMapType

The type of map to display.

Deprecated

var isZoomEnabled: Bool

A Boolean value that determines whether the user may use pinch gestures to zoom in and out of the map.

var isScrollEnabled: Bool

A Boolean value that determines whether the user may scroll around the map.

var isPitchEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s pitch information.

var isRotateEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s heading information.

var mapType: MKMapType

The type of data the map view displays.

Deprecated

### Manipulating the visible portion of the map

var region: MKCoordinateRegion

The area the map view displays.

func setRegion(MKCoordinateRegion, animated: Bool)

Changes the currently visible region, and optionally animates the change.

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

func setCenter(CLLocationCoordinate2D, animated: Bool)

Changes the center coordinate of the map, and optionally animates the change.

func showAnnotations([any MKAnnotation], animated: Bool)

Sets the visible region so that the map displays the specified annotations.

var visibleMapRect: MKMapRect

The area visible in the map view.

func setVisibleMapRect(MKMapRect, animated: Bool)

Changes the currently visible portion of the map, and optionally animates the change.

func setVisibleMapRect(MKMapRect, edgePadding: UIEdgeInsets, animated: Bool)

Changes the currently visible portion of the map, allowing you to specify additional space around the edges.

### Constraining the map view

func setCameraBoundary(MKMapView.CameraBoundary?, animated: Bool)

Sets the camera boundary for the map view, specifying whether to use animation.

var cameraBoundary: MKMapView.CameraBoundary?

The boundary of the area within which the map view’s center needs to remain.

func setCameraZoomRange(MKMapView.CameraZoomRange?, animated: Bool)

Sets the camera zoom range for the map view, specifying whether to use animation.

var cameraZoomRange: MKMapView.CameraZoomRange!

The zoom range to apply to the map view.

class CameraBoundary

A boundary of an area within which the map’s center needs to remain.

class CameraZoomRange

A camera zoom range that limits the distances to which the user can zoom.

### Configuring the map display

func setCamera(MKMapCamera, animated: Bool)

Changes the camera to use for determining the map’s viewing parameters, and optionally animates the change.

var camera: MKMapCamera

The camera to use for determining the appearance of the map.

var showsCompass: Bool

A Boolean value that indicates whether the map displays a compass control.

var showsPitchControl: Bool

A Boolean value that indicates whether the map displays the pitch control.

var showsScale: Bool

A Boolean value that indicates whether the map shows scale information.

var showsZoomControls: Bool

A Boolean value that indicates whether the map displays zoom controls.

var showsBuildings: Bool

A Boolean value that indicates whether the map displays extruded building information on supported map types.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear on the map.

Deprecated

var showsTraffic: Bool

A Boolean value that indicates whether the map displays traffic information.

Deprecated

### Displaying the user’s location

Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

### Annotating the map

var annotations: [any MKAnnotation]

The annotations associated with the map view.

func addAnnotation(any MKAnnotation)

Adds the specified annotation to the map view.

func addAnnotations([any MKAnnotation])

Adds an array of annotation objects to the map view.

func removeAnnotation(any MKAnnotation)

Removes the specified annotation object from the map view.

func removeAnnotations([any MKAnnotation])

Removes an array of annotation objects from the map view.

func annotations(in: MKMapRect) -> Set&lt;AnyHashable>

Returns the annotation objects within the specified map rectangle.

### Managing annotation selections

var annotationVisibleRect: CGRect

The visible rectangle where the map is displaying annotation views.

var selectedAnnotations: [any MKAnnotation]

The selected annotations.

func selectAnnotation(any MKAnnotation, animated: Bool)

Selects the specified annotation and displays a callout view for it.

func deselectAnnotation((any MKAnnotation)?, animated: Bool)

Deselects the specified annotation and hides its callout view.

### Creating annotation views

func register(AnyClass?, forAnnotationViewWithReuseIdentifier: String)

Registers an annotation view class that the map can create automatically.

func dequeueReusableAnnotationView(withIdentifier: String, for: any MKAnnotation) -> MKAnnotationView

Returns a reusable annotation view using the specified identifier with a specified existing annotation view, if possible.

func dequeueReusableAnnotationView(withIdentifier: String) -> MKAnnotationView?

Returns a reusable annotation view using its identifier.

func view(for: any MKAnnotation) -> MKAnnotationView?

Returns the annotation view associated with the specified annotation object, if any.

let MKMapViewDefaultAnnotationViewReuseIdentifier: String

The default reuse identifier for your map’s annotation views.

let MKMapViewDefaultClusterAnnotationViewReuseIdentifier: String

The default reuse identifier for the annotation view representing a cluster of annotations.

### Accessing overlays

var overlays: [any MKOverlay]

The overlay objects associated with the map view.

func overlays(in: MKOverlayLevel) -> [any MKOverlay]

Returns overlay objects in the specified level of the map.

func renderer(for: any MKOverlay) -> MKOverlayRenderer?

Returns the renderer object for drawing the contents of the specified overlay object.

enum MKOverlayLevel

Constants that indicate the position of overlays relative to other content.

func view(for: any MKOverlay) -> MKOverlayView

Returns the view associated with the overlay object, if any.

Deprecated

### Adding and inserting overlays

func addOverlay(any MKOverlay, level: MKOverlayLevel)

Adds the overlay object to the map at the specified level.

func addOverlays([any MKOverlay], level: MKOverlayLevel)

Adds an array of overlay objects to the map at the specified level.

func addOverlay(any MKOverlay)

Adds a single overlay object to the map.

func addOverlays([any MKOverlay])

Adds an array of overlay objects to the map.

func insertOverlay(any MKOverlay, at: Int, level: MKOverlayLevel)

Inserts an overlay object into the level at the specified index.

func insertOverlay(any MKOverlay, at: Int)

Inserts an overlay object into the list associated with the map.

func insertOverlay(any MKOverlay, above: any MKOverlay)

Inserts one overlay object above another.

func insertOverlay(any MKOverlay, below: any MKOverlay)

Inserts one overlay object below another.

func exchangeOverlay(any MKOverlay, with: any MKOverlay)

Exchanges the positions of two overlay objects.

func exchangeOverlay(at: Int, withOverlayAt: Int)

Exchanges the position of two overlay objects at the specified index.

### Removing overlays

func removeOverlay(any MKOverlay)

Removes a single overlay object from the map.

func removeOverlays([any MKOverlay])

Removes one or more overlay objects from the map.

### Converting map coordinates

func convert(CLLocationCoordinate2D, toPointTo: UIView?) -> CGPoint

Converts a map coordinate to a point in the specified view.

func convert(CGPoint, toCoordinateFrom: UIView?) -> CLLocationCoordinate2D

Converts a point in the specified view’s coordinate system to a map coordinate.

func convert(MKCoordinateRegion, toRectTo: UIView?) -> CGRect

Converts a map region to a rectangle in the specified view.

func convert(CGRect, toRegionFrom: UIView?) -> MKCoordinateRegion

Converts a rectangle in the specified view’s coordinate system to a map region.

### Adjusting map regions and rectangles

func regionThatFits(MKCoordinateRegion) -> MKCoordinateRegion

Adjusts the aspect ratio of the specified region to ensure that it fits in the map view’s frame.

func mapRectThatFits(MKMapRect) -> MKMapRect

Returns a centered map rectangle with the same aspect ratio as the map view’s frame.

func mapRectThatFits(MKMapRect, edgePadding: UIEdgeInsets) -> MKMapRect

Returns a centered, inset map rectangle with the same aspect ratio as the map view’s frame.

### Instance Properties

var selectableMapFeatures: MKMapFeatureOptions

The property that describes which selectable features the map responds to.

## Relationships

### Inherits From

- NSView
- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Essentials

Enabling Maps capability in Xcode

Configure your routing app to support providing directions.

Identifying unique locations with Place IDs

Obtain information about a point of interest that persists over its lifetime.

class MKMapItem

A point of interest on the map.

