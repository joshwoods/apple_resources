

- AppKit
-  Fonts 

API Collection

# Fonts

Manage the fonts used to display text.

## Overview

The NSFont and NSFontManager classes encapsulate and manage font families, sizes, and variations. The NSFont class defines a single object for each distinct font; for efficiency, these objects, which can be rather large, are shared by all the objects in your app. The NSFontPanel class defines the font specification panel that’s presented to the user.

## Topics

### Font Data

class NSFont

The representation of a font in an app.

class NSFontDescriptor

A dictionary of attributes that describe a font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

class NSFontAssetRequest

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

### Management

class NSFontManager

The center of activity for the font-conversion system.

class NSFontCollection

A font collection, which is a group of font descriptors taken together as a single object.

class NSMutableFontCollection

A mutable collection of font descriptors taken together as a single object.

struct NSFontCollectionOptions

Constants that support font collection management.

## See Also

### Text

Text Display

Display text and check spelling.

TextKit

Manage text storage and perform custom layout of text-based content in your app’s views.

Writing Tools

Add support for Writing Tools to your app’s text views.

