

- macOS Release Notes
-  AppKit Release Notes for macOS Monterey 12 

Article

# AppKit Release Notes for macOS Monterey 12

Update your apps to use new features, and test your apps against API changes.

## Overview

AppKit in macOS Monterey 12 includes new features, as well as API changes and deprecations.

### New Features

#### NSButton

- Buttons no longer highlight using the accent color when clicked. Before using any subclass that performs custom drawing, inspect the button cell’s doc://com.apple.documentation/documentation/appkit/nscell/1526141-interiorbackgroundstyle property to determine if the bezel draws in a normal or emphasized state.

- Buttons now support custom tinting with the bezelColor property. This property — previously applied only in the Touch Bar — now functions for all in-window buttons using the doc://com.apple.documentation/documentation/appkit/nsbuttontype/nsbuttontypemomentarypushin style.

#### NSSlider

- When clicking on the track, for linear sliders, circular sliders, or dial, the slider now animates to the new value.

- You can now tint sliders with colorful track fills using the trackFillColor property. This property now functions for all in-window sliders.

#### NSSegmentedControl

- Segmented controls now support custom tinting via the selectedSegmentBezelColor property. This property now functions for all in-window segmented control styles that draw colorful selected segments.

#### NSPopover

- NSPopover has a new animation when appearing and dismissing.

#### Symbol Images

- SF Symbols now support layered symbol images. Layered symbol images use an updated data format to annotate each path element of the symbol with a level in a hierarchy: primary, secondary, tertiary, and so on. At draw time, AppKit can assign different colors to each layer of the symbol using new APIs on NSImage.SymbolConfiguration. Many system-provided symbol images redesigned to include layered versions.

- NSImage.SymbolConfiguration now supports merging two configurations with applying(_:) method.

- NSImage now includes a read-only property, NSImage.SymbolConfiguration, for its current symbol configuration. You can use this property to configure other symbol images to match a reference image, or to merge an image’s existing configuration with a set of new configuration options.

#### Restorable State

- To enable secure coding for a restorable state, implement applicationSupportsSecureRestorableState(_:). When opted in:

  - The system requires classes passed to restorationClass to explicitly conform to NSWindowRestoration.

  - Set requiresSecureCoding to `true` and the decodingFailurePolicy to NSDecodingFailurePolicySetErrorAndReturn for any coder the following implementations or overrides use decodingFailurePolicy set to NSDecodingFailurePolicySetErrorAndReturn:

    - restoreWindow(withIdentifier:state:completionHandler:)

    - restoreWindow(withIdentifier:state:completionHandler:)

    - encodeRestorableState(with:)

    - encodeRestorableState(with:backgroundQueue:)

    - restoreState(with:)

    - restoreWindow(withIdentifier:state:completionHandler:)

    - encodeRestorableState(with:)

    - encodeRestorableState(with:backgroundQueue:)

    - restoreState(with:)

  - Additionally, restorableStateKeyPaths must only point at `NSSecureCoding`-compliant values and you need to implement allowedClasses(forRestorableStateKeyPath:) to specify the type of the object.

#### NSMenu

- The new user preference “Automatically hide and show the menu bar in full screen” in Dock & Menu Bar preferences is enabled by default. In macOS Monterey 12, the user can choose to disable this setting to always show the menu bar in full screen spaces. Standard full screen windows are resized to fit below the menu bar. Some apps assume a full screen-sized window, and don’t work well with this setting.

#### NSTableView

- 20-point spacing precedes each group row to make the separation between sections more visible. Source lists have a similar, but smaller, 13-point spacing. This applies to the NSTableView.Style.inset and NSTableView.Style.fullWidth effective styles in apps linked against the macOS 12 SDK. NSTableView.Style.plain doesn’t display the spacing.

- The floating group row transition — previously a push transition — instantly replaces the new floating group row. It occurs when the `x-height` of the group row’s label meets the bottom of a currently floating group row.

#### NSOutlineView

- The disclosure button now aligns with the cell view’s firstBaselineOffsetFromTop. The system overrides it in NSTableCellView so it matches the baseline of its textField (assuming `textfield` sets the baseline). Overriding the property and returning `0` reverts to the previous behavior.

- When collapsing several items, the selectionDidChangeNotification only posts once. Previously, it posted once per collapsed item.

#### NSOpenPanel

- Setting canChooseFiles to `false` automatically disabled files, but all of the directory contents were sent to panel(_:shouldEnable:) or panel:shouldShowFilename:. In macOS Monterey 12, files aren’t sent to the delegate methods unless `canChooseFiles` is `true`. In addition, file packages are excluded unless `treatsFilePackagesAsDirectoriesis` is `true`. This change allows optimization in the delegate method.

#### TextKit 2

- TextKit 2 introduces a new text layout engine and its associated API. You can use TextKit 2 alongside the existing TextKit API.

- NSTextContentStorage and NSTextLayoutManager are the two main controller objects superseding NSTextStorage and NSLayoutManager respectively. NSTextParagraph managed by `NSTextContentStorage` represents a paragraph of text. `NSTextLayoutManager` stores the layout information in its model objects: NSTextLayoutFragment and NSTextLineFragment.

- In TextKit 2, NSTextSelection encapsulates information associated with a text selection while NSTextSelectionNavigation manipulates and converts the selection object based on keyboard and mouse navigation actions.

