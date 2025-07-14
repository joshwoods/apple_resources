

- MapKit JS
- mapkit
- mapkit.Map
-  Handling map events 

Article

# Handling map events

Register an event lister for events that a map object dispatches.

## Overview

MapKit JS uses events that developers can implement to hook into points in the life cycle of the map, as well as user interactions. Your code can respond to events by registering an event listener.

Events have a `target` property. The `target` of an event is the object dispatching that event. When you add an event listener to a map, the target is the map itself. The `select` and `deselect` events have an annotation or overlay property that reports the selected or deselected item. The `single-tap`, `double-tap`, and `long-press` events have `pointOnPage` and `domEvents` properties that provide more data about the user interactions.

Event listeners receive a single argument that is an event object. The event objects are similar to native event objects, though calls to `event.preventDefault()` or `event.stopPropagation()` don’t halt some actions that trigger these events. Scrolling, zooming, and panning, as well as zooming or rotating after a long press, provide methods to halt or prevent interaction.

### Respond to map display events

MapKit JS sends events that allow you to respond to changes in the map display and a person’s interactions with the map and its controls.

`region-change-start`  
The map’s visible region is about to change.

`region-change-end`  
The map’s visible region finishes changing.

`rotation-start`  
The map’s rotation is about to change.

`rotation-end`  
The map’s rotation finishes changing.

`scroll-start`  
The map is about to scroll as a result of user interaction.

`scroll-end`  
The map finishes scrolling as a result of user interaction.

`zoom-start`  
The map is about to zoom as a result of user interaction.

`zoom-end`  
The map finishes zooming as a result of user interaction.

`map-type-change`  
A program event or a user interaction causes the map’s `type` (mapkit.Map.MapTypes) to change.

### Respond to annotation and overlay events

MapKit JS sends these events when a person’s interacts with the annotations and overlays you place on the map, use these to respond to these interactions by updating the map, or providing more informationation about the overlay or annotation the person interacts with.

`select`  
The user selects an annotation or an overlay. The event has either an `annotation` (mapkit.Annotation) property or an `overlay` (mapkit.Overlay) property, containing the selected annotation or overlay, respectively.

`deselect`  
The user deselects an annotation or an overlay. The event has either an `annotation` (mapkit.Annotation) property or an `overlay` (mapkit.Overlay) property, containing the selected annotation or overlay, respectively.

`drag-start`  
The user is starting to drag an annotation. The event has one property `annotation` (mapkit.Annotation), the dragged annotation.

`dragging`  
The user is dragging an annotation. The event has two properties. The first is an `annotation` (mapkit.Annotation) property, containing the dragged annotation. The second is a `coordinate` (mapkit.Coordinate) property, containing the coordinate of the annotation. This `coordinate` property is different from the annotation’s own coordinate property, which doesn’t update until the drag finishes.

`drag-end`  
The user finishes dragging an annotation. The event has one property `annotation` (mapkit.Annotation), the dragged annotation.

### Respond to user location events

MapKit JS sends these events that indicate changes in a person’s location. Use these events to adjust what the map displays or to trigger other responses in your app.

`user-location-change`  
MapKit JS sends this event when showsUserLocation is `true` and the map acquires the user’s location, or after an automatic update. The event object contains three properties. The first is the `coordinate` (mapkit.Coordinate) that contains the current location. The second is a `timestamp` (`Date`) that contains the time corresponding to the location acquisition. The third is a `floorLevel`, that returns either a floor number or `undefined` which represents the current floor the user is on, or `null` If the browser doesn’t expose this property.

`user-location-error`  
MapKit JS is unable to acquire the user’s location. The event has two properties. The first property is `code` (`Integer`), indicating why location acquisition failed. The second is a `message` (`String`) property, containing a human-readable string for the developer. This message isn’t for display to the user.

Because this feature implements the geolocation API for HTML 5, the error codes mirror that API’s error codes with one additional MapKit JS-specific error code:

`Error.PERMISSION_DENIED (1)` — The user refuses permission to obtain location information.

`Error.POSITION_UNAVAILABLE (2)` — The geolocation API returns an error.

`Error.TIMEOUT (3)` — The operation times out without acquiring the location.

`Error.MAPKIT_NOT_INITIALIZED (4)` — The system hasn’t initialized MapKit JS.

### Respond to map interaction events

MapKit JS sends these events when a person taps or presses on the map view. Use these events to adjust the map view, respond to the deselecting of overlays, or dragging or deselecting annotations.

`single-tap`  
A single tap occurs on the map outside an annotation or an overlay. If an annotation or an overlay is in a selected state when a single tap occurs, MapKit JS deselects the annotation or the overlay and dispatches a single-tap event.

`double-tap`  
A double tap occurs on the map without zooming the map.

`long-press`  
A long press occurs on the map outside an annotation. A long press may be the beginning of a panning or pinching gesture on the map. You can prevent the gesture from starting by calling the preventDefault() method of the event. Annotations need to be draggable to dispatch long-press events.

The event object that map interaction events return has the following two properties:

`pointOnPage`  
A DOM point with the coordinates `(x,` `y)` of the event on the page. You can use this property to derive a coordinate on the map using convertPointOnPageToCoordinate.

`domEvents`  
An array of DOM event objects listing the pertinent low-level events that led to the recognized gesture. You can inspect these and tailor the code to react according to the additional low-level events, such as modifier keys for the events.

## See Also

### Handling map events

addEventListener

Adds an event listener to handle events that user interactions and the framework trigger.

removeEventListener

Removes an event listener.

