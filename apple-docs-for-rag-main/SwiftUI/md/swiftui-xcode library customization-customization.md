

- SwiftUI
-  Xcode library customization 

# Xcode library customization

Expose custom views and modifiers in the Xcode library.

## Overview

You can add your custom SwiftUI views and view modifiers to Xcode’s library. This allows anyone developing your app or adopting your framework to access them by clicking the Library button (+) in Xcode’s toolbar. You can select and drag the custom library items into code, just like you would for system-provided items.

To add items to the library, create a structure that conforms to the LibraryContentProvider protocol and encapsulate any items you want to add as LibraryItem instances. Implement the doc://com.apple.documentation/documentation/DeveloperToolsSupport/LibraryContentProvider/views-25pdm computed property to add library items containing views. Implement the doc://com.apple.documentation/documentation/DeveloperToolsSupport/LibraryContentProvider/modifiers(base:)-4svii method to add items containing view modifiers. Xcode harvests items from all of the library content providers in your project as you work, and makes them available to you in its library.

## Topics

### Creating library items

protocol LibraryContentProvider

A source of Xcode library and code completion content.

struct LibraryItem

A single item to add to the Xcode library.

## See Also

### Tool support

Previews in Xcode

Generate dynamic, interactive previews of your custom views.

