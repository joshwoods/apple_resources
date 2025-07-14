

- XCUIAutomation
-  XCUIElementTypeQueryProvider 

Protocol

# XCUIElementTypeQueryProvider

A type that provides ready-made queries for locating descendant UI elements.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
protocol XCUIElementTypeQueryProvider
```

## Overview

Accessing the properties to get queries for descendant elements on an instance of a conforming class (such as an XCUIElement or XCUIElementQuery instance) is equivalent to calling descendants(matching:) for the corresponding element type.

## Topics

### Finding the first matching element

var firstMatch: XCUIElement

The first element that matches the query.

**Required**

### Querying descendant elements

var activityIndicators: XCUIElementQuery

A query that matches activity-indicator view elements.

**Required**

var alerts: XCUIElementQuery

A query that matches alert view elements.

**Required**

var browsers: XCUIElementQuery

A query that matches browser elements.

**Required**

var buttons: XCUIElementQuery

A query that matches button control elements.

**Required**

var cells: XCUIElementQuery

A query that matches cell elements.

**Required**

var checkBoxes: XCUIElementQuery

A query that matches checkbox control elements.

**Required**

var collectionViews: XCUIElementQuery

A query that matches collection view elements.

**Required**

var colorWells: XCUIElementQuery

A query that matches color-well elements.

**Required**

var comboBoxes: XCUIElementQuery

A query that matches combo-box control elements.

**Required**

var datePickers: XCUIElementQuery

A query that matches date-picker control elements.

**Required**

var decrementArrows: XCUIElementQuery

A query that matches decrement-arrow control elements.

**Required**

var dialogs: XCUIElementQuery

A query that matches dialog view elements.

**Required**

var disclosureTriangles: XCUIElementQuery

A query that matches disclosure-triangle control elements.

**Required**

var disclosedChildRows: XCUIElementQuery

A query that matches disclosed child row elements.

**Required**

var dockItems: XCUIElementQuery

A query that matches dock-item control elements.

**Required**

var drawers: XCUIElementQuery

A query that matches drawer elements.

**Required**

var grids: XCUIElementQuery

A query that matches grid view elements.

**Required**

var groups: XCUIElementQuery

A query that matches group elements.

**Required**

var handles: XCUIElementQuery

A query that matches handle control elements.

**Required**

var helpTags: XCUIElementQuery

A query that matches help-tag elements.

**Required**

var icons: XCUIElementQuery

A query that matches icon elements.

**Required**

var images: XCUIElementQuery

A query that matches image-view elements.

**Required**

var incrementArrows: XCUIElementQuery

A query that matches increment-arrow control elements.

**Required**

var keyboards: XCUIElementQuery

A query that matches keyboard elements.

**Required**

var keys: XCUIElementQuery

A query that matches key elements.

**Required**

var layoutAreas: XCUIElementQuery

A query that matches layout-area elements.

**Required**

var layoutItems: XCUIElementQuery

A query that matches layout-item elements.

**Required**

var levelIndicators: XCUIElementQuery

A query that matches level-indicator elements.

**Required**

var links: XCUIElementQuery

A query that matches link elements.

**Required**

var maps: XCUIElementQuery

A query that matches map-view elements.

**Required**

var mattes: XCUIElementQuery

A query that matches matte elements.

**Required**

var menuBarItems: XCUIElementQuery

A query that matches menu bar item elements.

**Required**

var menuBars: XCUIElementQuery

A query that matches menu bar elements.

**Required**

var menuButtons: XCUIElementQuery

A query that matches menu button elements.

**Required**

var menuItems: XCUIElementQuery

A query that matches menu item elements.

**Required**

var menus: XCUIElementQuery

A query that matches menu elements.

**Required**

var navigationBars: XCUIElementQuery

A query that matches navigation bar elements.

**Required**

var otherElements: XCUIElementQuery

A query that matches other view or control elements.

**Required**

var outlineRows: XCUIElementQuery

A query that matches outline row elements.

**Required**

var outlines: XCUIElementQuery

A query that matches outline view elements.

**Required**

var pageIndicators: XCUIElementQuery

A query that matches page-indicator control elements.

**Required**

var pickerWheels: XCUIElementQuery

A query that matches picker-wheel control elements.

**Required**

var pickers: XCUIElementQuery

A query that matches picker control elements.

**Required**

var popUpButtons: XCUIElementQuery

A query that matches popup-button control elements.

**Required**

var popovers: XCUIElementQuery

A query that matches popover view elements.

**Required**

var progressIndicators: XCUIElementQuery

A query that matches progress-indicator control elements.

**Required**

var radioButtons: XCUIElementQuery

A query that matches radio-button control elements.

**Required**

var radioGroups: XCUIElementQuery

A query that matches radio group elements.

**Required**

var ratingIndicators: XCUIElementQuery

A query that matches rating-indicator view elements.

**Required**

var relevanceIndicators: XCUIElementQuery

A query that matches relevance-indicator view elements.

**Required**

var rulerMarkers: XCUIElementQuery

A query that matches ruler marker elements.

**Required**

var rulers: XCUIElementQuery

A query that matches ruler view elements.

**Required**

var scrollBars: XCUIElementQuery

A query that matches scroll bar elements.

**Required**

var scrollViews: XCUIElementQuery

A query that matches scroll view elements.

**Required**

var searchFields: XCUIElementQuery

A query that matches search field elements.

**Required**

var secureTextFields: XCUIElementQuery

A query that matches secure text field elements.

**Required**

var segmentedControls: XCUIElementQuery

A query that matches segmented control elements.

**Required**

var sheets: XCUIElementQuery

A query that matches sheet elements.

**Required**

var sliders: XCUIElementQuery

A query that matches slider elements.

**Required**

var splitGroups: XCUIElementQuery

A query that matches split group elements.

**Required**

var splitters: XCUIElementQuery

A query that matches splitter elements.

**Required**

var staticTexts: XCUIElementQuery

A query that matches static-text view elements.

**Required**

var statusBars: XCUIElementQuery

A query that matches status bar elements.

**Required**

var statusItems: XCUIElementQuery

A query that matches status item elements.

**Required**

var steppers: XCUIElementQuery

A query that matches stepper elements.

**Required**

var switches: XCUIElementQuery

A query that matches switch control elements.

**Required**

var tabBars: XCUIElementQuery

A query that matches tab bar elements.

**Required**

var tabGroups: XCUIElementQuery

A query that matches tab group elements.

**Required**

var tableColumns: XCUIElementQuery

A query that matches table column elements.

**Required**

var tableRows: XCUIElementQuery

A query that matches table row elements.

**Required**

var tables: XCUIElementQuery

A query that matches table elements.

**Required**

var tabs: XCUIElementQuery

A query that matches tab elements.

**Required**

var textFields: XCUIElementQuery

A query that matches text field elements.

**Required**

var textViews: XCUIElementQuery

A query that matches text view elements.

**Required**

var timelines: XCUIElementQuery

A query that matches timeline view elements.

**Required**

var toggles: XCUIElementQuery

A query that matches toggle control elements.

**Required**

var toolbarButtons: XCUIElementQuery

A query that matches toolbar button elements.

**Required**

var toolbars: XCUIElementQuery

A query that matches toolbar elements.

**Required**

var touchBars: XCUIElementQuery

A query that matches touch bar elements.

**Required**

var valueIndicators: XCUIElementQuery

A query that matches value indicator elements.

**Required**

var webViews: XCUIElementQuery

A query that matches web view elements.

**Required**

var windows: XCUIElementQuery

A query that matches window elements.

**Required**

## Relationships

### Conforming Types

- XCUIApplication
- XCUIElement
- XCUIElementQuery
- XCUISiriService

## See Also

### UI element queries

class XCUIElementQuery

An object that defines the search criteria a test uses to identify UI elements.

