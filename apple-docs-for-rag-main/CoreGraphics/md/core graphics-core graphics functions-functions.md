

- Core Graphics
-  Core Graphics Functions 

API Collection

# Core Graphics Functions

## Topics

### Functions

func CGAcquireDisplayFadeReservation(CGDisplayReservationInterval, UnsafeMutablePointer&lt;CGDisplayFadeReservationToken>?) -> CGError

Reserves the fade hardware for a specified time interval.

func CGAssociateMouseAndMouseCursorPosition(boolean_t) -> CGError

Connects or disconnects the mouse and cursor while an application is in the foreground.

func CGBeginDisplayConfiguration(UnsafeMutablePointer&lt;CGDisplayConfigRef?>?) -> CGError

Begins a new set of display configuration changes.

func CGCancelDisplayConfiguration(CGDisplayConfigRef?) -> CGError

Cancels a set of display configuration changes.

func CGCaptureAllDisplays() -> CGError

Obtains exclusive use of all active displays, preventing other applications and system services from using the display or changing its configuration.

func CGCaptureAllDisplaysWithOptions(CGCaptureOptions) -> CGError

Captures all attached displays, using the specified options.

func CGCompleteDisplayConfiguration(CGDisplayConfigRef?, CGConfigureOption) -> CGError

Completes a set of display configuration changes.

func CGConfigureDisplayFadeEffect(CGDisplayConfigRef?, CGDisplayFadeInterval, CGDisplayFadeInterval, Float, Float, Float) -> CGError

Modifies the settings of the built-in fade effect that occurs during a display configuration.

func CGConfigureDisplayMirrorOfDisplay(CGDisplayConfigRef?, CGDirectDisplayID, CGDirectDisplayID) -> CGError

Changes the configuration of a mirroring set.

func CGConfigureDisplayMode(CGDisplayConfigRef?, CGDirectDisplayID, CFDictionary?) -> CGError

Configures the display mode of a display.

Deprecated

func CGConfigureDisplayOrigin(CGDisplayConfigRef?, CGDirectDisplayID, Int32, Int32) -> CGError

Configures the origin of a display relative to the global display coordinate space.

func CGConfigureDisplayStereoOperation(CGDisplayConfigRef?, CGDirectDisplayID, boolean_t, boolean_t) -> CGError

Enables or disables stereo operation for a display, as part of a display configuration.

func CGConfigureDisplayWithDisplayMode(CGDisplayConfigRef?, CGDirectDisplayID, CGDisplayMode?, CFDictionary?) -> CGError

Configures the display mode of a display.

func CGCursorIsDrawnInFramebuffer() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is drawn in framebuffer memory.

Deprecated

func CGCursorIsVisible() -> boolean_t

Returns a Boolean value indicating whether the mouse cursor is visible.

Deprecated

func CGDirectDisplayCopyCurrentMetalDevice(CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

func CGDisplayAvailableModes(CGDirectDisplayID) -> CFArray?

Returns information about the currently available display modes.

Deprecated

func CGDisplayBestModeForParameters(CGDirectDisplayID, Int, Int, Int, UnsafeMutablePointer&lt;boolean_t>?) -> CFDictionary?

Returns information about the display mode closest to a specified depth and screen size.

Deprecated

func CGDisplayBestModeForParametersAndRefreshRate(CGDirectDisplayID, Int, Int, Int, CGRefreshRate, UnsafeMutablePointer&lt;boolean_t>?) -> CFDictionary?

Returns information about the display mode closest to a specified depth, screen size, and refresh rate.

Deprecated

func CGDisplayBounds(CGDirectDisplayID) -> CGRect

Returns the bounds of a display in the global display coordinate space.

func CGDisplayCapture(CGDirectDisplayID) -> CGError

Obtains exclusive use of a display, preventing other applications and system services from using the display or changing its configuration.

func CGDisplayCaptureWithOptions(CGDirectDisplayID, CGCaptureOptions) -> CGError

Obtains exclusive use of a display for an application using the options you specify.

func CGDisplayCopyAllDisplayModes(CGDirectDisplayID, CFDictionary?) -> CFArray?

Returns information about the currently available display modes.

func CGDisplayCopyColorSpace(CGDirectDisplayID) -> CGColorSpace

Returns the color space for a display.

func CGDisplayCopyDisplayMode(CGDirectDisplayID) -> CGDisplayMode?

Returns information about a display’s current configuration.

func CGDisplayCreateImage(CGDirectDisplayID) -> CGImage?

Returns an image containing the contents of the specified display.

Deprecated

func CGDisplayCreateImage(CGDirectDisplayID, rect: CGRect) -> CGImage?

Returns an image containing the contents of a portion of the specified display.

Deprecated

func CGDisplayCurrentMode(CGDirectDisplayID) -> CFDictionary?

Returns information about the current display mode.

Deprecated

func CGDisplayFade(CGDisplayFadeReservationToken, CGDisplayFadeInterval, CGDisplayBlendFraction, CGDisplayBlendFraction, Float, Float, Float, boolean_t) -> CGError

Performs a single fade operation.

func CGDisplayFadeOperationInProgress() -> boolean_t

Returns a Boolean value indicating whether a fade operation is currently in progress.

Deprecated

func CGDisplayGammaTableCapacity(CGDirectDisplayID) -> UInt32

Returns the capacity, or number of entries, in the gamma table for a display.

func CGDisplayGetDrawingContext(CGDirectDisplayID) -> CGContext?

Returns a graphics context suitable for drawing to a captured display.

func CGDisplayHideCursor(CGDirectDisplayID) -> CGError

Hides the mouse cursor, and increments the hide cursor count.

func CGDisplayIDToOpenGLDisplayMask(CGDirectDisplayID) -> CGOpenGLDisplayMask

Maps a display ID to an OpenGL display mask.

func CGDisplayIOServicePort(CGDirectDisplayID) -> io_service_t

Returns the I/O Kit service port of the specified display.

Deprecated

func CGDisplayIsActive(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is active.

func CGDisplayIsAlwaysInMirrorSet(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is always in a mirroring set.

func CGDisplayIsAsleep(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is sleeping (and is therefore not drawable).

func CGDisplayIsBuiltin(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is built-in, such as the internal display in portable systems.

func CGDisplayIsCaptured(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is captured.

Deprecated

func CGDisplayIsInHWMirrorSet(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is in a hardware mirroring set.

func CGDisplayIsInMirrorSet(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is in a mirroring set.

func CGDisplayIsMain(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is the main display.

func CGDisplayIsOnline(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is connected or online.

func CGDisplayIsStereo(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether a display is running in a stereo graphics mode.

func CGDisplayMirrorsDisplay(CGDirectDisplayID) -> CGDirectDisplayID

For a secondary display in a mirroring set, returns the primary display.

var pixelEncoding: CFString?

Returns the pixel encoding of the specified display mode.

Deprecated

var height: Int

Returns the height of the specified display mode.

var ioDisplayModeID: Int32

Returns the I/O Kit display mode ID of the specified display mode.

var ioFlags: UInt32

Returns the I/O Kit flags of the specified display mode.

var pixelWidth: Int

var refreshRate: Double

Returns the refresh rate of the specified display mode.

class var typeID: CFTypeID

Returns the type identifier of Quartz display modes.

var width: Int

Returns the width of the specified display mode.

func isUsableForDesktopGUI() -> Bool

Returns a Boolean value indicating whether the specified display mode is usable for a desktop graphical user interface.

func CGDisplayModelNumber(CGDirectDisplayID) -> UInt32

Returns the model number of a display monitor.

func CGDisplayMoveCursorToPoint(CGDirectDisplayID, CGPoint) -> CGError

Moves the mouse cursor to a specified point relative to the upper-left corner of the display.

func CGDisplayPixelsHigh(CGDirectDisplayID) -> Int

Returns the display height in pixel units.

func CGDisplayPixelsWide(CGDirectDisplayID) -> Int

Returns the display width in pixel units.

func CGDisplayPrimaryDisplay(CGDirectDisplayID) -> CGDirectDisplayID

Returns the primary display in a hardware mirroring set.

func CGDisplayRegisterReconfigurationCallback(CGDisplayReconfigurationCallBack?, UnsafeMutableRawPointer?) -> CGError

Registers a callback function to be invoked whenever a local display is reconfigured.

func CGDisplayRelease(CGDirectDisplayID) -> CGError

Releases a captured display.

func CGDisplayRemoveReconfigurationCallback(CGDisplayReconfigurationCallBack?, UnsafeMutableRawPointer?) -> CGError

Removes the registration of a callback function that’s invoked whenever a local display is reconfigured.

func CGDisplayRestoreColorSyncSettings()

Restores the gamma tables to the values in the user’s ColorSync display profile.

func CGDisplayRotation(CGDirectDisplayID) -> Double

Returns the rotation angle of a display in degrees.

func CGDisplayScreenSize(CGDirectDisplayID) -> CGSize

Returns the width and height of a display in millimeters.

func CGDisplaySerialNumber(CGDirectDisplayID) -> UInt32

Returns the serial number of a display monitor.

func CGDisplaySetDisplayMode(CGDirectDisplayID, CGDisplayMode?, CFDictionary?) -> CGError

Switches a display to a different mode.

func CGDisplaySetStereoOperation(CGDirectDisplayID, boolean_t, boolean_t, CGConfigureOption) -> CGError

Immediately enables or disables stereo operation for a display.

func CGDisplayShowCursor(CGDirectDisplayID) -> CGError

Decrements the hide cursor count, and shows the mouse cursor if the count is `0`.

init?(display: CGDirectDisplayID, outputWidth: Int, outputHeight: Int, pixelFormat: Int32, properties: CFDictionary?, handler: CGDisplayStreamFrameAvailableHandler?)

Creates a new display stream to be used with a `CFRunloop`.

Deprecated

init?(dispatchQueueDisplay: CGDirectDisplayID, outputWidth: Int, outputHeight: Int, pixelFormat: Int32, properties: CFDictionary?, queue: dispatch_queue_t, handler: CGDisplayStreamFrameAvailableHandler?)

Creates a new display stream whose updates are delivered to a dispatch queue.

Deprecated

var runLoopSource: CFRunLoopSource?

Gets the run loop source for a display stream.

Deprecated

func start() -> CGError

Tells a stream to start sending updates.

Deprecated

func stop() -> CGError

Tells a stream to stop sending updates.

Deprecated

init?(mergedUpdateFirstUpdate: CGDisplayStreamUpdate?, secondUpdate: CGDisplayStreamUpdate?)

Combines two updates into a new update that includes the metadata for both source updates.

Deprecated

var dropCount: Int

Returns the number of frames that have been dropped since the last call to your update handler.

Deprecated

func getMovedRectsDelta(dx: UnsafeMutablePointer&lt;CGFloat>, dy: UnsafeMutablePointer&lt;CGFloat>)

Return the movement delta values for a single update.

Deprecated

func getRects(CGDisplayStreamUpdateRectType, rectCount: UnsafeMutablePointer&lt;Int>) -> UnsafePointer&lt;CGRect>?

Returns an array of rectangles that describe where the frame has changed since the previous frame.

Deprecated

class var typeID: CFTypeID

Returns the type identifier of a Quartz display stream update.

Deprecated

func CGDisplaySwitchToMode(CGDirectDisplayID, CFDictionary?) -> CGError

Switches a display to a different mode.

Deprecated

func CGDisplayUnitNumber(CGDirectDisplayID) -> UInt32

Returns the logical unit number of a display.

func CGDisplayUsesOpenGLAcceleration(CGDirectDisplayID) -> boolean_t

Returns a Boolean value indicating whether Quartz is using OpenGL-based window acceleration (Quartz Extreme) to render in a display.

func CGDisplayVendorNumber(CGDirectDisplayID) -> UInt32

Returns the vendor number of the specified display’s monitor.

func CGEnableEventStateCombining(boolean_t) -> CGError

Enables or disables the merging of actual key and mouse state with the application-specified state in a synthetic event.

Deprecated

init?(source: CGEventSource?)

Returns a new Quartz event.

func copy() -> CGEvent?

Returns a copy of an existing Quartz event.

init?(withDataAllocator: CFAllocator?, data: CFData?)

Returns a Quartz event created from a flattened data representation of the event.

init?(keyboardEventSource: CGEventSource?, virtualKey: CGKeyCode, keyDown: Bool)

Returns a new Quartz keyboard event.

init?(mouseEventSource: CGEventSource?, mouseType: CGEventType, mouseCursorPosition: CGPoint, mouseButton: CGMouseButton)

Returns a new Quartz mouse event.

init?(event: CGEvent?)

Returns a Quartz event source created from an existing Quartz event.

func getDoubleValueField(CGEventField) -> Double

Returns the floating-point value of a field in a Quartz event.

var flags: CGEventFlags

Returns the event flags of a Quartz event.

func getIntegerValueField(CGEventField) -> Int64

Returns the integer value of a field in a Quartz event.

var location: CGPoint

Returns the location of a Quartz mouse event.

var timestamp: CGEventTimestamp

Returns the timestamp of a Quartz event.

var type: CGEventType

Returns the event type of a Quartz event (left mouse down, for example).

class var typeID: CFTypeID

Returns the type identifier for the opaque type `CGEventRef`.

var unflippedLocation: CGPoint

Returns the location of a Quartz mouse event.

func keyboardGetUnicodeString(maxStringLength: Int, actualStringLength: UnsafeMutablePointer&lt;Int>?, unicodeString: UnsafeMutablePointer&lt;UniChar>?)

Returns the Unicode string associated with a Quartz keyboard event.

func keyboardSetUnicodeString(stringLength: Int, unicodeString: UnsafePointer&lt;UniChar>?)

Sets the Unicode string associated with a Quartz keyboard event.

func post(tap: CGEventTapLocation)

Posts a Quartz event into the event stream at a specified location.

func postToPSN(processSerialNumber: UnsafeMutableRawPointer?)

Posts a Quartz event into the event stream for a specific application.

func postToPid(pid_t)

func setDoubleValueField(CGEventField, value: Double)

Sets the floating-point value of a field in a Quartz event.

func setIntegerValueField(CGEventField, value: Int64)

Sets the integer value of a field in a Quartz event.

func setSource(CGEventSource?)

Sets the event source of a Quartz event.

class func buttonState(CGEventSourceStateID, button: CGMouseButton) -> Bool

Returns a Boolean value indicating the current button state of a Quartz event source.

class func counterForEventType(CGEventSourceStateID, eventType: CGEventType) -> UInt32

Returns a count of events of a given type seen since the window server started.

init?(stateID: CGEventSourceStateID)

Returns a Quartz event source created with a specified source state.

class func flagsState(CGEventSourceStateID) -> CGEventFlags

Returns the current flags of a Quartz event source.

var keyboardType: CGEventSourceKeyboardType

Returns the keyboard type to be used with a Quartz event source.

func getLocalEventsFilterDuringSuppressionState(CGEventSuppressionState) -> CGEventFilterMask

Returns the mask that indicates which classes of local hardware events are enabled during event suppression.

var pixelsPerLine: Double

Gets the scale of pixels per line in a scrolling event source.

var sourceStateID: CGEventSourceStateID

Returns the source state associated with a Quartz event source.

class var typeID: CFTypeID

Returns the type identifier for the opaque type `CGEventSourceRef`.

var userData: Int64

Returns the 64-bit user-specified data for a Quartz event source.

class func keyState(CGEventSourceStateID, key: CGKeyCode) -> Bool

Returns a Boolean value indicating the current keyboard state of a Quartz event source.

class func secondsSinceLastEventType(CGEventSourceStateID, eventType: CGEventType) -> CFTimeInterval

Returns the elapsed time since the last event for a Quartz event source.

func setLocalEventsFilterDuringSuppressionState(CGEventFilterMask, state: CGEventSuppressionState)

Sets the mask that indicates which classes of local hardware events are enabled during event suppression.

class func tapCreate(tap: CGEventTapLocation, place: CGEventTapPlacement, options: CGEventTapOptions, eventsOfInterest: CGEventMask, callback: CGEventTapCallBack, userInfo: UnsafeMutableRawPointer?) -> CFMachPort?

Creates an event tap.

class func tapCreateForPSN(processSerialNumber: UnsafeMutableRawPointer, place: CGEventTapPlacement, options: CGEventTapOptions, eventsOfInterest: CGEventMask, callback: CGEventTapCallBack, userInfo: UnsafeMutableRawPointer?) -> CFMachPort?

Creates an event tap for a specified process.

class func tapCreateForPid(pid: pid_t, place: CGEventTapPlacement, options: CGEventTapOptions, eventsOfInterest: CGEventMask, callback: CGEventTapCallBack, userInfo: UnsafeMutableRawPointer?) -> CFMachPort?

class func tapEnable(tap: CFMachPort, enable: Bool)

Enables or disables an event tap.

class func tapIsEnabled(tap: CFMachPort) -> Bool

Returns a Boolean value indicating whether an event tap is enabled.

func tapPostEvent(CGEventTapProxy?)

Posts a Quartz event from an event tap into the event stream.

func CGGetActiveDisplayList(UInt32, UnsafeMutablePointer&lt;CGDirectDisplayID>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Provides a list of displays that are active for drawing.

func CGGetDisplayTransferByFormula(CGDirectDisplayID, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?) -> CGError

Gets the coefficients of the gamma transfer formula for a display.

func CGGetDisplayTransferByTable(CGDirectDisplayID, UInt32, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;CGGammaValue>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Gets the values in the RGB gamma tables for a display.

func CGGetDisplaysWithOpenGLDisplayMask(CGOpenGLDisplayMask, UInt32, UnsafeMutablePointer&lt;CGDirectDisplayID>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Provides a list of displays that corresponds to the bits set in an OpenGL display mask.

func CGGetDisplaysWithPoint(CGPoint, UInt32, UnsafeMutablePointer&lt;CGDirectDisplayID>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Provides a list of online displays with bounds that include the specified point.

func CGGetDisplaysWithRect(CGRect, UInt32, UnsafeMutablePointer&lt;CGDirectDisplayID>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Gets a list of online displays with bounds that intersect the specified rectangle.

func CGGetEventTapList(UInt32, UnsafeMutablePointer&lt;CGEventTapInformation>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Gets a list of currently installed event taps.

func CGGetLastMouseDelta() -> (x: Int32, y: Int32)

Reports the change in mouse position since the last mouse movement event received by the application.

func CGGetOnlineDisplayList(UInt32, UnsafeMutablePointer&lt;CGDirectDisplayID>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Provides a list of displays that are online (active, mirrored, or sleeping).

var utType: CFString?

The Universal Type Identifier for the image.

func CGInhibitLocalEvents(boolean_t) -> CGError

Turns off local hardware events in the current session.

Deprecated

func CGMainDisplayID() -> CGDirectDisplayID

Returns the display ID of the main display.

func CGOpenGLDisplayMaskToDisplayID(CGOpenGLDisplayMask) -> CGDirectDisplayID

Maps an OpenGL display mask to a display ID.

func CGPointEqualToPoint(CGPoint, CGPoint) -> Bool

Returns whether two points are equal.

Deprecated

func CGPostKeyboardEvent(CGCharCode, CGKeyCode, boolean_t) -> CGError

Synthesizes a low-level keyboard event on the local machine.

Deprecated

func CGRegisterScreenRefreshCallback(CGScreenRefreshCallback, UnsafeMutableRawPointer?) -> CGError

Registers a callback function to be invoked when local displays are refreshed or modified.

Deprecated

func CGReleaseAllDisplays() -> CGError

Releases all captured displays.

func CGReleaseDisplayFadeReservation(CGDisplayFadeReservationToken) -> CGError

Releases a display fade reservation, and unfades the display if needed.

func CGReleaseScreenRefreshRects(UnsafeMutablePointer&lt;CGRect>?)

Deallocates a list of rectangles that represent changed areas on local displays.

Deprecated

func CGRestorePermanentDisplayConfiguration()

Restores the permanent display configuration settings for the current user.

func CGScreenRegisterMoveCallback(CGScreenUpdateMoveCallback, UnsafeMutableRawPointer?) -> CGError

Registers a callback function to be invoked when an area of the display is moved.

Deprecated

func CGScreenUnregisterMoveCallback(CGScreenUpdateMoveCallback, UnsafeMutableRawPointer?)

Removes a previously registered callback function invoked when an area of the display is moved.

Deprecated

func CGSessionCopyCurrentDictionary() -> CFDictionary?

Returns information about the caller’s window server session.

func CGSetDisplayTransferByByteTable(CGDirectDisplayID, UInt32, UnsafePointer&lt;UInt8>, UnsafePointer&lt;UInt8>, UnsafePointer&lt;UInt8>) -> CGError

Sets the byte values in the 8-bit RGB gamma tables for a display.

func CGSetDisplayTransferByFormula(CGDirectDisplayID, CGGammaValue, CGGammaValue, CGGammaValue, CGGammaValue, CGGammaValue, CGGammaValue, CGGammaValue, CGGammaValue, CGGammaValue) -> CGError

Sets the gamma function for a display by specifying the coefficients of the gamma transfer formula.

func CGSetDisplayTransferByTable(CGDirectDisplayID, UInt32, UnsafePointer&lt;CGGammaValue>?, UnsafePointer&lt;CGGammaValue>?, UnsafePointer&lt;CGGammaValue>?) -> CGError

Sets the color gamma function for a display by specifying the values in the RGB gamma tables.

func CGSetLocalEventsFilterDuringSuppressionState(CGEventFilterMask, CGEventSuppressionState) -> CGError

Filters local hardware events from the keyboard and mouse during the short interval after a synthetic event is posted.

Deprecated

func CGSetLocalEventsSuppressionInterval(CFTimeInterval) -> CGError

Sets the time interval in seconds that local hardware events are suppressed after posting a synthetic event.

Deprecated

func CGShieldingWindowID(CGDirectDisplayID) -> CGWindowID

Returns the window ID of the shield window for a captured display.

func CGShieldingWindowLevel() -> CGWindowLevel

Returns the window level of the shield window for a captured display.

func CGSizeEqualToSize(CGSize, CGSize) -> Bool

Returns whether two sizes are equal.

Deprecated

func CGUnregisterScreenRefreshCallback(CGScreenRefreshCallback, UnsafeMutableRawPointer?)

Removes a previously registered callback function invoked when local displays are refreshed or modified.

Deprecated

func CGWaitForScreenRefreshRects(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CGRect>?>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Waits for screen refresh operations.

Deprecated

func CGWaitForScreenUpdateRects(CGScreenUpdateOperation, UnsafeMutablePointer&lt;CGScreenUpdateOperation>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CGRect>?>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;CGScreenUpdateMoveDelta>?) -> CGError

Waits for screen update operations.

Deprecated

func CGWarpMouseCursorPosition(CGPoint) -> CGError

Moves the mouse cursor without generating events.

func CGWindowLevelForKey(CGWindowLevelKey) -> CGWindowLevel

Returns the window level that corresponds to one of the standard window types.

func CGWindowListCopyWindowInfo(CGWindowListOption, CGWindowID) -> CFArray?

Generates and returns information about the selected windows in the current user session.

func CGWindowListCreateDescriptionFromArray(CFArray?) -> CFArray?

Generates and returns information about windows with the specified window IDs.

func CGWindowListCreateImage(CGRect, CGWindowListOption, CGWindowID, CGWindowImageOption) -> CGImage?

Returns a composite image based on a dynamically generated list of windows.

Deprecated

init?(windowListFromArrayScreenBounds: CGRect, windowArray: CFArray, imageOption: CGWindowImageOption)

Returns a composite image of the specified windows.

Deprecated

func CGWindowServerCFMachPort() -> CFMachPort?

Returns a Core Foundation Mach port (CFMachPort) that corresponds to the macOS window server.

Deprecated

func CGWindowServerCreateServerPort() -> CFMachPort?

func acos(CGFloat) -> CGFloat

func acosh(CGFloat) -> CGFloat

func asin(CGFloat) -> CGFloat

func asinh(CGFloat) -> CGFloat

func atan(CGFloat) -> CGFloat

func atan2(CGFloat, CGFloat) -> CGFloat

func atanh(CGFloat) -> CGFloat

func cbrt(CGFloat) -> CGFloat

func copysign(CGFloat, CGFloat) -> CGFloat

func cos(CGFloat) -> CGFloat

func cosh(CGFloat) -> CGFloat

func erf(CGFloat) -> CGFloat

func erfc(CGFloat) -> CGFloat

func exp(CGFloat) -> CGFloat

func exp2(CGFloat) -> CGFloat

func expm1(CGFloat) -> CGFloat

func fdim(CGFloat, CGFloat) -> CGFloat

func fmax(CGFloat, CGFloat) -> CGFloat

func fmin(CGFloat, CGFloat) -> CGFloat

func hypot(CGFloat, CGFloat) -> CGFloat

func ilogb(CGFloat) -> Int

func CGColorSpaceCreateLinearized(CGColorSpace) -> CGColorSpace?

init?(src: CGColorSpace, dst: CGColorSpace)

Creates a conversion between two specified color spaces.

func j0(CGFloat) -> CGFloat

func j1(CGFloat) -> CGFloat

func jn(Int, CGFloat) -> CGFloat

func ldexp(CGFloat, Int) -> CGFloat

func lgamma(CGFloat) -> (CGFloat, Int)

func log(CGFloat) -> CGFloat

func log10(CGFloat) -> CGFloat

func log1p(CGFloat) -> CGFloat

func log2(CGFloat) -> CGFloat

func logb(CGFloat) -> CGFloat

func nan(String) -> CGFloat

func nearbyint(CGFloat) -> CGFloat

func nextafter(CGFloat, CGFloat) -> CGFloat

func pow(CGFloat, CGFloat) -> CGFloat

func remquo(CGFloat, CGFloat) -> (CGFloat, Int)

func rint(CGFloat) -> CGFloat

func sin(CGFloat) -> CGFloat

func sinh(CGFloat) -> CGFloat

func tan(CGFloat) -> CGFloat

func tanh(CGFloat) -> CGFloat

func tgamma(CGFloat) -> CGFloat

var localEventsSuppressionInterval: CFTimeInterval

Returns the interval that local hardware events may be suppressed following the posting of a Quartz event.

var pixelHeight: Int

class var typeID: CFTypeID

Returns the type identifier of a Quartz display stream.

Deprecated

class var typeID: CFTypeID

Returns the Core Foundation type identifier for a color conversion info data type.

func y0(CGFloat) -> CGFloat

func y1(CGFloat) -> CGFloat

func yn(Int, CGFloat) -> CGFloat

func CGAffineTransformMake(CGFloat, CGFloat, CGFloat, CGFloat, CGFloat, CGFloat) -> CGAffineTransform

Returns an affine transformation matrix constructed from values you provide.

func CGColorSpaceCopyBaseColorSpace(CGColorSpace) -> CGColorSpace

func CGColorSpaceCreateCopyWithStandardRange(CGColorSpace) -> CGColorSpace

func CGColorSpaceCreateExtended(CGColorSpace) -> CGColorSpace?

func CGColorSpaceCreateExtendedLinearized(CGColorSpace) -> CGColorSpace?

func CGColorSpaceCreateWithColorSyncProfile(ColorSyncProfile?, CFDictionary?) -> CGColorSpace?

func CGColorSpaceIsHLGBased(CGColorSpace) -> Bool

func CGColorSpaceIsPQBased(CGColorSpace) -> Bool

func CGColorSpaceUsesITUR_2100TF(CGColorSpace) -> Bool

func CGContextDrawConicGradient(CGContext, CGGradient?, CGPoint, CGFloat)

func CGContextGetEDRTargetHeadroom(CGContext) -> Float

func CGConvertColorDataWithFormat(Int, Int, UnsafeMutableRawPointer!, CGColorDataFormat, UnsafeMutableRawPointer!, CGColorDataFormat, CFDictionary!) -> Bool

func CGEnableEventStateCombining(boolean_t) -> CGError

Enables or disables the merging of actual key and mouse state with the application-specified state in a synthetic event.

Deprecated

func CGErrorSetCallback(CGErrorCallback!)

func CGImageCreateCopyWithContentHeadroom(Float, CGImage) -> CGImage?

func CGInhibitLocalEvents(boolean_t) -> CGError

Turns off local hardware events in the current session.

Deprecated

func CGPDFArrayApplyBlock(CGPDFArrayRef, CGPDFArrayApplierBlock, UnsafeMutableRawPointer?)

func CGPDFContextBeginTag(CGContext, CGPDFTagType, CFDictionary)

func CGPDFContextEndTag(CGContext)

func CGPDFContextSetIDTree(CGContext, CGPDFDictionaryRef)

func CGPDFContextSetOutline(CGContext, CFDictionary?)

func CGPDFContextSetPageTagStructureTree(CGContext, CFDictionary)

func CGPDFContextSetParentTree(CGContext, CGPDFDictionaryRef)

func CGPDFDictionaryApplyBlock(CGPDFDictionaryRef, CGPDFDictionaryApplierBlock, UnsafeMutableRawPointer?)

func CGPDFScannerStop(CGPDFScannerRef)

func CGPointMake(CGFloat, CGFloat) -> CGPoint

Returns a point with the specified coordinates.

func CGPointMakeWithDictionaryRepresentation(CFDictionary, UnsafeMutablePointer&lt;CGPoint>) -> Bool

Fills in a point using the contents of the specified dictionary.

func CGPostKeyboardEvent(CGCharCode, CGKeyCode, boolean_t) -> CGError

Synthesizes a low-level keyboard event on the local machine.

Deprecated

func CGPreflightListenEventAccess() -> Bool

func CGPreflightPostEventAccess() -> Bool

func CGPreflightScreenCaptureAccess() -> Bool

func CGRectMake(CGFloat, CGFloat, CGFloat, CGFloat) -> CGRect

Returns a rectangle with the specified coordinate and size values.

func CGRectMakeWithDictionaryRepresentation(CFDictionary, UnsafeMutablePointer&lt;CGRect>) -> Bool

Fills in a rectangle using the contents of the specified dictionary.

func CGRegisterScreenRefreshCallback(CGScreenRefreshCallback, UnsafeMutableRawPointer?) -> CGError

Registers a callback function to be invoked when local displays are refreshed or modified.

Deprecated

func CGReleaseScreenRefreshRects(UnsafeMutablePointer&lt;CGRect>?)

Deallocates a list of rectangles that represent changed areas on local displays.

Deprecated

func CGRequestListenEventAccess() -> Bool

func CGRequestPostEventAccess() -> Bool

func CGRequestScreenCaptureAccess() -> Bool

func CGScreenRegisterMoveCallback(CGScreenUpdateMoveCallback, UnsafeMutableRawPointer?) -> CGError

Registers a callback function to be invoked when an area of the display is moved.

Deprecated

func CGScreenUnregisterMoveCallback(CGScreenUpdateMoveCallback, UnsafeMutableRawPointer?)

Removes a previously registered callback function invoked when an area of the display is moved.

Deprecated

func CGSetLocalEventsFilterDuringSuppressionState(CGEventFilterMask, CGEventSuppressionState) -> CGError

Filters local hardware events from the keyboard and mouse during the short interval after a synthetic event is posted.

Deprecated

func CGSetLocalEventsSuppressionInterval(CFTimeInterval) -> CGError

Sets the time interval in seconds that local hardware events are suppressed after posting a synthetic event.

Deprecated

func CGSizeMake(CGFloat, CGFloat) -> CGSize

Returns a size with the specified dimension values.

func CGSizeMakeWithDictionaryRepresentation(CFDictionary, UnsafeMutablePointer&lt;CGSize>) -> Bool

Fills in a size using the contents of the specified dictionary.

func CGUnregisterScreenRefreshCallback(CGScreenRefreshCallback, UnsafeMutableRawPointer?)

Removes a previously registered callback function invoked when local displays are refreshed or modified.

Deprecated

func CGVectorMake(CGFloat, CGFloat) -> CGVector

Returns a vector with the specified dimension values.

func CGWaitForScreenRefreshRects(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CGRect>?>?, UnsafeMutablePointer&lt;UInt32>?) -> CGError

Waits for screen refresh operations.

Deprecated

func CGWaitForScreenUpdateRects(CGScreenUpdateOperation, UnsafeMutablePointer&lt;CGScreenUpdateOperation>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CGRect>?>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;CGScreenUpdateMoveDelta>?) -> CGError

Waits for screen update operations.

Deprecated

var accessPermissions: CGPDFAccessPermissions

func applyWithBlock((UnsafePointer&lt;CGPathElement>) -> Void)

var byteOrderInfo: CGImageByteOrderInfo

var containsImageSpecificToneMappingMetadata: Bool

var contentHeadroom: Float

func convert(width: Int, height: Int, to: UnsafeMutableRawPointer, format: CGColorBufferFormat, from: UnsafeRawPointer, format: CGColorBufferFormat, options: CFDictionary?) -> Bool

func copyPropertyList() -> CFPropertyList?

Returns a copy of the color space’s properties.

var info: UnsafeMutableRawPointer?

init(genericGrayGamma2_2Gray: CGFloat, alpha: CGFloat)

Creates a color in the Generic gray color space with a gamma ramp of 2.2.

init?(headroom: Float, width: Int, height: Int, bitsPerComponent: Int, bitsPerPixel: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: CGBitmapInfo, provider: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

init?(iccData: CFTypeRef)

Creates an ICC-based color space using the ICC profile contained in the specified data.

init?(optionsSrc: CGColorSpace, dst: CGColorSpace, options: CFDictionary?)

init?(propertyListPlist: CFPropertyList)

Creates a color space from a property list.

init?(scrollWheelEvent2Source: CGEventSource?, units: CGScrollEventUnit, wheelCount: UInt32, wheel1: Int32, wheel2: Int32, wheel3: Int32)

init?(src: CGColorSpace, srcHeadroom: Float, dst: CGColorSpace, dstHeadroom: Float, toneMapping: CGToneMapping, options: CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

func isHDR() -> Bool

var name: UnsafePointer&lt;CChar>

var outline: CFDictionary?

var pixelFormatInfo: CGImagePixelFormatInfo

func resetClip()

func setEDRTargetHeadroom(Float) -> Bool

var shouldToneMap: Bool

func CGColorSpaceUsesExtendedRange(CGColorSpace) -> Bool

## See Also

### Reference

Core Graphics Structures

Core Graphics Enumerations

Core Graphics Constants

Core Graphics Data Types

