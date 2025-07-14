

- macOS Release Notes
- macOS Mojave 10.14 Release Notes
-  AppKit Release Notes for macOS 10.14 

Article

# AppKit Release Notes for macOS 10.14

Update your apps to use new features, and test your apps against API changes.

## Overview

AppKit in macOS 10.14 includes new features, as well as API changes and deprecations. For information about earlier releases, see AppKit Release Notes for macOS 10.13.

Pay special attention to the additions and changes described in *Supporting Dark Mode* and *Swift and Objective-C API Enhancements*.

### Supporting Dark Mode

In macOS 10.14, users can choose to adopt a systemwide light or dark appearance. The Light (aqua) appearance is the default appearance. When an app links on the macOS 10.14 SDK, it’s automatically opted in to supporting the dark appearance, with its NSApp inheriting the darkAqua appearance from System Preferences. You can override the automatic behavior to explicitly opt in to or opt out of supporting Dark mode using the optional `NSRequiresAquaSystemAppearance` `Info.plist` key: Setting the key to `NO` allows an app to support Dark mode regardless of link check; setting it to `YES` forces it to opt out. Use the `Info.plist` key to opt out only before you audit an app for compatibility with Dark mode. You may not be able to opt out of supporting Dark mode in future versions of macOS.

For more information, see Supporting Dark Mode in Your Interface and Choosing a Specific Appearance for Your macOS App.

#### Named Image and Color Support in Dark Mode

When you add custom image and color sets to an asset catalog, you can define appearance-sensitive variants to be used when an image is shown in a context with that appearance. Images and colors that you create using the existing NSImage init(named:) and NSColor init(named:) initializers maintain a dynamic connection to the named asset catalog set and don’t need to be recreated when the appearance changes. When an image is drawn or a color is resolved, the instance queries the current appearance to determine the correct image or color to use.

The asset catalog is backward compatible with older releases, where the Light (aqua) appearance asset is used.

#### Automatic NSVisualEffectView Appearance Inheritance

For apps linked against the macOS 10.14 SDK, NSVisualEffectView automatically uses the correct vibrant NSAppearance as its appearance, based on the appearance of its superview. For example, if its superview uses the aqua appearance, NSVisualEffectView uses vibrantLight. As a result, you shouldn’t explicitly set the appearance of the NSVisualEffectView, either in code or in Interface Builder. Explicitly setting the appearance was necessary in earlier versions of macOS.

Using the automatic appearance is especially important for supporting Dark mode where, for example, setting the vibrantLight appearance makes the NSVisualEffectView visually clash with the rest of your app.

#### New NSVisualEffectView Materials

NSVisualEffectView.Material includes new semantic materials in macOS 10.14. Semantic materials are like semantic colors: their names describe where they are used, not what they look like. They might look different in different system appearances.

##### Desktop-Tinted Materials

Three of the new semantic materials use a color tinting effect based on the user’s desktop picture when in Dark mode. In the aqua appearance, the new materials currently look the same as their corresponding NSColor:

- NSVisualEffectView.Material.contentBackground looks the same as controlBackgroundColor in the aqua appearance.

- NSVisualEffectView.Material.windowBackground looks the same as windowBackgroundColor in the aqua appearance.

- NSVisualEffectView.Material.underPageBackground looks the same as underPageBackgroundColor in the aqua appearance.

If your app sets its background or fill colors according to one of the following conditions, AppKit now instead adds the corresponding NSVisualEffectView material:

- The backgroundColor of a window is set to windowBackgroundColor.

- The backgroundColor of a table view, scroll view, or collection view is set to controlBackgroundColor or underPageBackgroundColor.

- The fillColor of a custom NSBox is set to controlBackgroundColor, windowBackgroundColor, or underPageBackgroundColor.

If your app sets its background or fill colors differently, you can use NSVisualEffectView directly to add the material.

To avoid drawing issues, apps linked on macOS SDKs prior to 10.14 are opted out of the tinting effect when a table view’s background color is set to controlBackgroundColor and the table view overrides isOpaque.

#### Deprecation of Nonsemantic Materials

The following nonsemantic materials are now deprecated:

- NSVisualEffectView.Material.light

- NSVisualEffectView.Material.dark

- NSVisualEffectView.Material.mediumLight

- NSVisualEffectView.Material.ultraDark

- NSVisualEffectView.Material.appearanceBased

#### Printing Views

When you print an NSView through an NSPrintOperation, its appearance now gets temporarily replaced by the aqua appearance during rendering. This is done to avoid printing with an inherited dark appearance. The NSView instance’s own appearance property—if it’s set—is left unaltered, so it remains possible to print views with a nonstandard appearance, if desired.

Use separate, off-screen views to print the contents of on-screen windows. To avoid altering the contents of on-screen windows, the darkAqua appearance isn’t replaced when printing views that are simultaneously hosted in a window.

#### Appearance-Aware Credits

You make the credits area match the appearance of an app by supplying the credits as an attributed string or by placing a `Credits.rtf` or `Credits.rtfd` in your app’s bundle. Use the proper system colors, like textColor, linkColor, and labelColor, to make text display correctly in any appearance.

If you use `.rtf` or `.rtfd` files to supply text for the credits area, the file must be saved using macOS 10.14 (beta 5 or later) to receive the appearance-aware treatment. If you create the file `.rtf` or `.rtfd` files on an earlier version of macOS, the appearance-aware treatment is only applied if the file contains only black text with no background color.

### Accent Colors

macOS 10.14 introduces a new user preference called the *accent color*. Use this color to tint the colorful parts of system controls, selection materials, and focus rings. A new system color, controlAccentColor, draws dynamically using the user’s current preferred accent color. Your app’s views are automatically redrawn when the accent color changes.

NSColor uses the new withSystemEffect(_:) method to include built-in effects for states like NSColor.SystemEffect.pressed, NSColor.SystemEffect.disabled, and NSColor.SystemEffect.rollover. This method produces a dynamically modified version of the color, applying effects that are tuned for the appearance of the current drawing context. These effects update automatically as the appearance context changes.

Named NSColor objects defined in asset catalogs (`.xcassets`) can now vary their resolved color values based on the current NSAppearance at draw time. You use the asset catalog editor to specialize the color definition for the Dark and Increased Contrast modes. The resulting named colors are fully dynamic, and adapt to their context without requiring an explicit refresh.

### Rich Text Authoring

When you save a rich text file (RTF) in macOS 10.14, the names of the NSColor values that represent the colors in the rich text are saved in the file in addition to the individual evaluated components. When you open a rich text file that was saved in macOS 10.14, the named color values are used as the source of color information instead of the components.

Note

Named colors aren’t saved when you use document formats other than RTF or Rich Text Format Directory (RTFD).

The new appearance document attribute controls how the underlying unnamed colors are represented when you save rich text. If you omit this attribute in a document, named colors use the aqua appearance.

### Swift and Objective-C API Enhancements

AppKit’s Swift interface is improved in macOS 10.14 in pursuit of greater clarity, consistency, concision, and a native Swift feel. In many cases, these enhancements go in hand with refinements to the corresponding Objective-C APIs. The changes include formalizing informal protocols; moving enumerations to a common-prefix identifier convention; hoisting Swift declarations into appropriate local namespaces; renaming some functions for Swift; replacing functions with computed properties; adding setters for some previously read-only array-valued properties; and similar enhancements that are discussed in these release notes.

#### Automatically Sized Instances of NSToolbarItem

Beginning in apps linked on the macOS 10.14 SDK, if an NSToolbarItem doesn’t have its minSize and maxSize properties set, these values are calculated automatically by AppKit using constraints, similar to how the size properties for NSTouchBarItem are set. (Previously, if the item’s minimum and maximum size properties weren’t set, the size of the containing view was used.) You can use constraints to define both a minimum and maximum size that will be calculated by AppKit.

For example, you can create the following constraints to give the view a minimum width of 100 and a maximum width of 200:

```
view.widthAnchor.constraint(greaterThanOrEqualToConstant: 100).isActive = true
view.widthAnchor.constraint(lessThanOrEqualToConstant: 200).isActive = true
```

The same applies for height. Omitting a minimum width or height constraint will use the view’s intrinsic content size, which is automatically adjusted for localization purposes for controls.

If the view being measured has an undefined height or width, the view’s frame size is used instead.

#### Centered Toolbar Items

NSToolbar has a new centeredItemIdentifier property that lets a single item be centered absolutely in the window, assuming space allows. When the window shrinks, or more items are added by the user, the highest priority is to have the most items visible. As a result, centering is broken first by pushing the item off center to the left or right as necessary.

To center multiple items together, you can specify an NSToolbarItemGroup object’s itemIdentifier as the centeredItemIdentifier of the NSToolbar. The centered item must still appear in the toolbar delegate’s allowed item identifiers array.

#### Layer-Backed Views

Windows in apps linked against the macOS 10.14 SDK are displayed using Core Animation when the app is running in macOS 10.14. This *doesn’t* mean that all views are layer-backed; rather, it means that all views are either layer-backed or draw into a shared layer with other layers.

This change should be mostly invisible to most apps, but you might notice one or more subtle changes as a result.

Views that depend on drawing in the same backing store as their ancestors or lower-ordered siblings may find that they are instead drawing in separate layers. Views shouldn’t rely on being able to draw into the same backing store as their ancestors; instead, those ancestors should change as required. For example, to affect the background of a window, use the NSWindow properties isOpaque and backgroundColor.

Views that implicitly depend on being redrawn when an ancestor, descendant, or intersecting sibling is redrawn may not be redrawn. As before, if a view needs to be redrawn, set its needsDisplay property to `true`.

Views that return `true` from wantsUpdateLayer will typically be given an exclusive layer, even if the view’s wantsLayer property is set to `false`. Apps targeting macOS 10.14 should prefer the wantsUpdateLayer property over the wantsLayer property.

#### Deprecated Underline Styles and Their Replacements

The following NSUnderlineStyle members are soft deprecated as of macOS 10.14. *Soft deprecation* means that the members are still available, but that they’re slated for deprecation and using them in new code is discouraged.

- `NSUnderlinePatternSolid` is replaced by NSUnderlineStylePatternSolid.

- `NSUnderlinepatternDot` is replaced by patternDot.

- `NSUnderlinepatternDash` is replaced by patternDash.

- `NSUnderlinepatternDashDot` is replaced by patternDashDot.

- `NSUnderlinepatternDashDotDot` is replaced by patternDashDotDot.

- `NSUnderlineByWord` is replaced by byWord.

#### NSTableRowView Background Style Inference

For apps linked on macOS 10.14 and later, the value of an NSTableRowView instance’s interiorBackgroundStyle property no longer infers its emphasized style using its backgroundColor property. Instead, the interiorBackgroundStyle property defaults to NSView.BackgroundStyle.normal, but becomes emphasized when it’s selected and focused by the table. If you want to use the emphasized style outside the context of selection, manually set backgroundStyle or override interiorBackgroundStyle to return NSView.BackgroundStyle.emphasized.

#### NSTextView Enhancements

Four new convenience factory methods for NSTextView in macOS 10.14 are similar to ones for other NSControl subclasses. These include fieldEditor(), scrollableDocumentContentTextView(), scrollablePlainDocumentContentTextView(), and scrollableTextView().

Each new method is purpose-oriented and returns an instance preconfigured for the target usage. For example, the scrollableTextView() method instantiates a text view packaged inside an NSScrollView that is best used as a UI component like the Comments section in Finder and Calendar inspector panels. Use the fieldEditor() method when you’re instantiating a custom field editor for an NSTextField in order to modify the default behavior. The scrollableDocumentContentTextView() and scrollablePlainDocumentContentTextView() methods display document contents configured for user documents, like the plain text and rich text modes in TextEdit.

Other than scrollableDocumentContentTextView(), all factory methods use the semantic colors and the default appearance to support Dark mode.

Use the new performValidatedReplacement(in:with:) method with NSTextView to modify text as edited by the user. It validates the proposed change with shouldChangeText(in:replacementString:) and didChangeText() so that the system services associated with the text view—such as spelling and undo—are properly handled. The method also substitutes attributes absent from the attributed string with the corresponding keys inside the typing attributes. This helps you focus on attributes you’re interested in without worrying about keeping track of essential attributes like foregroundColor in Dark mode.

#### NSTextField Background Style Inference

For apps linked on macOS 10.14 and later, NSTextField instances in an NSTableRowView no longer infer the NSView.BackgroundStyle.emphasized interior background style for their associated NSTextFieldCell instances based on the background color. The inferred style now depends on whether you set drawsBackground.

Text fields that *don’t* draw their own backgrounds now infer interiorBackgroundStyle based on backgroundStyle. These text fields get the emphasized interior background style by default if they’re inside a selected table row. Setting backgroundStyle for these text fields propagates that style to the interior background style.

Text fields that *do* draw their own backgrounds get the NSView.BackgroundStyle.normal interior background style by default even if they’re inside a selected table row. If you want the emphasized interior background style, override interiorBackgroundStyle on the text field’s cell to return NSView.BackgroundStyle.emphasized.

#### NSRulerView and NSTextFinder View Sizing

For apps linked on macOS 10.14, the document of an NSScrollView can scroll under the associated horizontal and vertical NSRulerView or findBarView. This means that the NSClipView is sized and positioned under those accessories, and that will be reflected in the clip view’s contentInsets.

If you’re writing a document view class that observes the containing clip view’s size to determine its own size, take these contentInsets into account when you’re determining the document size, to avoid it being larger than the inset document area.

#### Action Extensions as Quick Actions

Your action extensions can now appear as Quick Actions in Finder and Touch Bar. Use the following keys to enable this new behavior:

- `NSExtensionServiceAllowsFinderPreviewItem`: set this to `YES` for the action extension to show up as a Quick Action in Finder.

- `NSExtensionServiceFinderPreviewLabel`: the label to use for the action. If you don’t specify a value, the bundle’s display name is used.

- `NSExtensionServiceFinderPreviewIconName`: the icon to use for the action in Finder. The name is looked up in the action extension’s bundle, followed by the system. The icon should be a template image. If you don’t specify a value, a default icon is displayed.

- `NSExtensionServiceAllowsTouchBarItem`: set this to `YES` for the action extension to show up as a Quick Action on Touch Bar.

- `NSExtensionServiceTouchBarLabel`: the label to use for the action. If you don’t specify a value, the bundle’s display name is used.

- `NSExtensionServiceTouchBarIconName`: the icon to use for the action on Touch Bar. The name is looked up in the action extension’s bundle, followed by the system. The icon should be a template image. If you don’t specify a value, a default icon is displayed.

- `NSExtensionServiceTouchBarBezelColorName`: the color of the button’s bezel on Touch Bar. The name is looked up in the action extension’s bundle in the default asset catalog. The color should be a system color. If you don’t specify a value, a default color is used instead.

The NSItemProvider class’s suggestedName property is now available on macOS, and the NSExtensionItem class’s attachments property is now explicitly typed as an array of NSItemProvider instances.

#### Drag and Drop

If you’re using certain deprecated APIs in apps linked on macOS 10.14, you’ll see two kinds of exceptions being thrown.

If you encounter an exception about dragging multiple files using the deprecated NSFilenamesPboardType and dragging API, adopt the following APIs depending on your usage:

- drag(_:at:offset:event:pasteboard:source:slideBack:): Adopt NSDraggingSession and use URL instances instead of string file paths.

- tableView:writeRows:toPasteboard: or tableView(_:writeRowsWith:to:): Adopt tableView(_:pasteboardWriterForRow:) and return URL instances or `nil` if the row shouldn’t be dragged.

- collectionView(_:writeItemsAt:to:): Adopt collectionView(_:pasteboardWriterForItemAt:) and return URL instances or `nil` if the row shouldn’t be dragged.

If you encounter an exception noting that “there must be 1 draggingItem per pasteboardItem,” you need to ensure that the number of pasteboard items you add is the same as the number of drag items you’re using. The same exception occurs if you use the deprecated drag and drop API. Update your drag and drop code to NSDraggingSession or collectionView(_:pasteboardWriterForItemAt:) to avoid the exception in that case.

#### API Changes

- NSApplication: NSApplication now conforms to the NSAppearanceCustomization protocol, which you use to query, override, and key-value observe the global NSAppearance of your app.

  The showHelp(_:) method now searches the list of bundles registered via the NSHelpManager registerBooks(in:) method as a new fallback when Help content isn’t otherwise found.

- NSBezierPath: New replacement identifiers are declared for the NSBezierPath.ElementType, NSBezierPath.LineCapStyle, NSBezierPath.LineJoinStyle, and NSBezierPath.WindingRule constants in `NSBezierPath.h`. The new identifiers follow a common-prefix convention that matches modern Cocoa API design practice and also produces more concise identifiers in AppKit’s Swift interfaces. For example, the NSBezierPath.LineJoinStyle.miter, NSBezierPath.LineJoinStyle.round, and NSBezierPath.LineJoinStyle.bevel cases of the NSBezierPath.LineJoinStyle enumeration are more concise when used in Swift.

- NSBox: The borderColor, borderWidth, cornerRadius, and fillColor properties now support animation via the animator proxy. These properties only apply to boxes whose boxType is set to NSBox.BoxType.custom.

- NSButton: You can use the new contentTintColor property to provide a base color for template images and text inside borderless buttons. For buttons that look different only while they’re being pushed—including button with types such as NSButton.ButtonType.momentaryLight—this color is used in all states. Toggle buttons use the color to indicate the on state. AppKit automatically derives additional states—like pressed and disabled—by altering your color using an appearance-appropriate modifier. The content tint color doesn’t apply to non-template images or attributed titles.

- NSCollectionView: The moveSection(_:toSection:) method fails for sections containing more than one item, and may raise a parameter exception if internal cached state isn’t initialized on macOS 10.12 and later. Use deleteSections(_:) and insertSections(_:) instead.

- NSCollectionViewLayout and NSCollectionViewFlowLayout: As part of the system appearance changes in macOS 10.14, collapsed sections in an NSCollectionViewFlowLayout are now displayed flat rather than fanned out at the ends. Initiation of an item drag, when some of the selected items are outside the currently instantiated item set, now consults the layout for unknown item frames, preventing exceptions that could otherwise occur due to empty draggingFrame values. In previous releases, it was possible for an NSCollectionViewLayout to be asked for its collectionViewContentSize before it received a prepare() message. This is fixed in macOS 10.14. An issue that could prevent item selection in apps linked on macOS prior to 10.10 is fixed in macOS 10.14.

- NSColorSpace: NSColorSpace now supports Objective-C weak references. NSColorSpace instances can now be stored in weak instance variables or collections.

- NSDatePicker: The NSDatePicker.ElementFlags, NSDatePicker.Mode, and NSDatePicker.Style types have new identifiers that follow a more modern common-prefix naming convention. As a result, their Swift counterparts are now more concise. For example, the possible values for NSDatePicker.Style are now NSDatePicker.Style.textFieldAndStepper, NSDatePicker.Style.clockAndCalendar, and NSDatePicker.Style.textField.

- NSDisableScreenUpdates() and NSEnableScreenUpdates(): These two functions are now deprecated. They were used to force the window server to avoid redrawing certain parts of the screen.

  As of macOS 10.11, these methods are no longer necessary. AppKit view and windowing operations are committed transactionally. This satisfies most needs for visual atomicity without any extra code. If you have an extra-strong need for guaranteed visual atomicity—for example, to ensure atomicity while running the run loop or calling out to client code—use NSAnimationContext instead.

- NSDraggingInfo: NSDraggingInfo APIs that were previously declared as getter methods are now declared as read-only properties, which means they can now be accessed as properties in Swift, without needing the parenthesized `()` function call syntax.

  The draggedImage property is superseded by the NSDraggingItem API, and is now deprecated.

- NSEditor: The NSEditor protocol’s `commitEditingAndReturnError()` method is renamed, in Swift, to commitEditingWithoutPresentingError() to more clearly reflect the purpose of this method and the fact that in Swift it throws an error rather than returning an error.

- NSImageView: You can use the new contentTintColor property to provide a custom fill color for template images being presented inside borderless image views.

- NSLayoutManager: NSLayoutManager now renders the spellingState and textAlternatives consistently between macOS and iOS by using flat circles. The NSLayoutManager.GlyphProperty structure is now declared using the `NS_OPTIONS` macro instead of the `NS_ENUM` macro. The NSLayoutManager.ControlCharacterAction structure is now declared using the `NS_OPTIONS` macro instead of the `NS_ENUM` macro. For information about how these macros affect how an Objective-C type is imported in Swift, see Grouping Related Objective-C Constants.

- NSMenu: The items property is now settable. Its new setter is implemented based on the existing API funnel points for adding, inserting, and removing items to allow for potential overrides of those methods.

  Don’t entirely reset the contents of a menu while it’s open.

- NSOpenGLGlobalOption: The NSOpenGLGlobalOption structure is now declared using the `NS_ENUM` macro, and appears in Swift as a native structure.

- NSOutlineView: Swift value types provided as items to an NSOutlineView instance using methods such as insertItems(at:inParent:withAnimation:) need to be made both Equatable and Hashable. For more information, see Adopting Common Protocols.

  These conformances let NSOutlineView correctly compare items so that performance is optimal and methods like row(forItem:) can correctly find the stored item internally.

- NSPrintInfo.PaginationMode: The NSPrintInfo.PaginationMode enumeration is modernized to use a common prefix for its identifier names. In Swift, the possible values for NSPrintInfo.PaginationMode are now written as NSPrintInfo.PaginationMode.automatic, NSPrintInfo.PaginationMode.fit, and NSPrintInfo.PaginationMode.clip.

- NSResponder: The `try(toPerform:with:)` method is renamed tryToPerform(_:with:) in Swift.

- NSSearchField: NSSearchField now centers the placeholder text and looking glass icon as a single unit rather than centering the placeholder text first.

- NSSecureCoding: NSBezierPath, NSGradient, NSShadow, and NSSound now adopt NSSecureCoding.

- NSTabView: The tabViewItems property is now settable. Its new setter is implemented based on the existing API funnel points for adding, inserting, and removing items to allow for potential overrides of those methods.

- NSTableViewDelegate and NSOutlineViewDelegate: Returning a value of -1 from either the tableView(_:heightOfRow:) or doc://com.apple.documentation/documentation/AppKit/NSOutlineViewdelegate/1531870-outlineView delegate method uses the standard size for that row. If the row is a group row, the system-defined height for group rows is used. Otherwise, the height defined by the rowHeight is used. It’s still possible to provide a custom height for group rows from these delegate methods.

  If these methods aren’t implemented and only the rowHeight property is used, group rows always default to using the system defined height.

- NSUnderlineStyle: The NSUnderlineStyle structure is now declared using the `NS_OPTIONS` macro instead of the `NS_ENUM` macro.

- NSView: The `mouse(_:in:)` method is renamed isMousePoint(_:in:) in Swift.

- NSViewController: The `childViewControllers` property is renamed children in Swift. Many NSViewController methods for managing and presenting child controllers are likewise renamed for greater conciseness in Swift by removing redundant occurrences of `ViewController`.

- NSWindow: NSWindow declares a new NSWindow.PersistableFrameDescriptor type that encapsulates the results returned for the `stringWithSavedFrame` property. The `setFrameFrom(_:)` method is renamed setFrame(from:), and now takes an NSWindow.PersistableFrameDescriptor parameter. In hand with this change, the read-only `stringWithSavedFrame` property is renamed frameDescriptor in Swift.

### New Macros in AppKit Headers

Uses of `NS_STRING_ENUM` in AppKit headers are replaced by the more general `NS_TYPED_ENUM`. Similarly, uses of `NS_EXTENSIBLE_STRING_ENUM` in AppKit headers are replaced by the more modern and general `NS_TYPED_EXTENSIBLE_ENUM`. The new macros are equivalent to the ones they replace, so this is purely a switch to more modern naming conventions that should have no effect on compiled code.

Some uses of `NS_EXTENSIBLE_STRING_ENUM` are replaced by `NS_SWIFT_BRIDGED_TYPEDEF`. This new macro supports exporting the affected typedefs as Swift type aliases, as described below.

#### Removed Macro Applications

To support simpler and more concise usage in Swift, some AppKit string enumeration types now import to Swift as type aliases of String, instead of as structures. This eliminates the need for you to explicitly wrap String constants in cases like:

```
let nib = NSNib(nibNamed: NSNib.Name("Inspector"), bundle: nil)
```

Calls to these APIs can now be simplified to:

```
let nib = NSNib(nibNamed: "Inspector", bundle: nil)
```

This change was made for types with values that pass through the API to drive things like named asset lookup.

The affected typedefs are now declared using the new `NS_SWIFT_BRIDGED_TYPEDEF` qualifier, whereas in macOS 10.13 they were declared as `NS_EXTENSIBLE_STRING_ENUM` types.

### New Formal Protocols

AppKit now provides formal `@protocol` declarations for sets of methods that were formerly declared as *informal protocols*, which are categories on NSObject or some other class. Here are the new protcols:

- NSColorChanging

- NSFontChanging

- NSEditor

- NSMenuItemValidation

- NSPasteboardTypeOwner

- NSStandardKeyBindingResponding

- NSToolbarItemValidation

- NSViewToolTipOwner

- NSViewLayerContentScaleDelegate

Some of AppKit’s classes conform to these new formal protocols. The doc://com.apple.documentation/documentation/AppKit/NSControlTextEditingDelegate/3005176-controlTextDidBeginEditing, doc://com.apple.documentation/documentation/AppKit/NSControlTextEditingDelegate/3005178-controlTextDidEndEditing, and doc://com.apple.documentation/documentation/AppKit/NSControlTextEditingDelegate/3005177-controlTextDidChange methods, which were previously declared using informal protocols, have also been added to the existing NSControlTextEditingDelegate protocol as optional methods.

To help ensure source compatibility, the corresponding informal protocol declarations remain in AppKit’s headers alongside the new formal protocols. Adopt the new formal protocols where appropriate, as the informal protocol declarations might be deprecated in a future release.

### Typesetter Behavior Changes

The default typesetter behavior has changed for apps that are compiled with the macOS 10.14 SDK and have a deployment target of macOS 10.14: String drawing now uses NSLayoutManager.TypesetterBehavior.behavior_10_4 for all AppKit controls. Previously, only some portions of AppKit used NSLayoutManager.TypesetterBehavior.behavior_10_4, and other portions used NSLayoutManager.TypesetterBehavior.behavior_10_2_WithCompatibility.

The typesetter behavior change corrects a long-standing floating-point rounding error that resulted in an extra pixel being added to the default ascender, so text might now measure 1 point smaller than it did previously. Reevaluate any of your code that hardcodes heights or makes manual adjustments to the y-origin of cells or text baselines based on the new text measurement.

### Identifying New and Deprecated APIs in Headers

New APIs in headers are marked with availability macros that include references to macOS 10.14:

```
```

Deprecated APIs are marked with the `NS_DEPRECATED_MAC` macro:

```
```

Deprecation macros might also include a suggested replacement API:

```
```

### Checking macOS and AppKit Versions

To check for new features provided by Cocoa frameworks at runtime, look for a given new class or method dynamically. Don’t use it if it isn’t there.

In Swift, you use `#available`:

```
if #available(macOS 10.14, *) {
    // Code for macOS 10.14 or later.
} else {
    // Code for versions earlier than 10.14.
}
```

Starting in Xcode 9, you use `@available` from Objective-C:

```
if (@available(macOS 10.14, *)) {
    // Code for macOS 10.14 or later
} else {
    // Code for versions earlier than 10.14.
}
```

You can also use the global constant `NSAppKitVersionNumber` (`NSAppKitVersion.`current in Swift).

```
let current = NSAppKitVersion.current

if current 

Note

In Foundation, you use the NSFoundationVersionNumber global variable.

Unlike most AppKit software updates, macOS 10.10 software updates incremented the AppKit major version, which accounts for the specific treatment of macOS10_10_Max in the example above. Other special cases or situations for version checking are discussed in the release notes as appropriate. Some individual headers may also declare an AppKit version number where some bug fix or functionality is available in a given update, for example:

```
```

### Checking for Backward Compatibility

You can check for the version of the system an app was built against, and if your app is running on an older system, modify its behavior to be more compatible. You do this in cases where incompatibility problems are predicted or discovered; most of these problems are described in these release notes.

Typically, the system detects how an app was built by looking at the “SDK” entry in the app’s Mach-O header. When you relink your app against the latest SDK, you might notice different behaviors, some of which might cause incompatibilities. In these cases, because the app is being rebuilt, you should address these issues at the same time. For this reason, if you’re doing a small incremental update of your app to address a few bugs, it’s usually best to continue building on the same build environment and libraries used originally.

In some cases, AppKit provides `defaults`—preferences—that you can use to get the old or new behavior, independent of what system an app was linked against. These preferences are often provided for debugging purposes only; in some cases you can use the preferences to globally modify the behavior of an app by registering the values. When you set one of these preferences, do so somewhere very early in your app’s startup process using methods like register(defaults:).

