

- AppKit
-  NSPrinter 

Class

# NSPrinter

An object that describes a printer’s capabilities.

macOS

``` source
class NSPrinter
```

## Overview

NSPrinter provides information about a printer; it does not modify printer attributes or control a printing job. A printer object can be constructed by specifying either the printer name or the make and model of an available printer. Typically, Cocoa apps don’t create NSPrinter objects; instead, the printing system uses these objects to support the printing jobs and when it shows users a list of printers.

## Topics

### Creating the Printer Object

init?(name: String)

Creates and returns a printer object initialized with the specified printer name.

init?(type: NSPrinter.TypeName)

Creates and returns a printer object initialized to the first available printer with the specified make and model information.

### Getting General Printer Information

class var printerNames: [String]

Returns the names of all available printers.

class var printerTypes: [NSPrinter.TypeName]

Returns descriptions of the makes and models of all available printers.

struct TypeName

The type you use to describe a printer’s make and model.

### Getting Attributes

var name: String

The printer’s name.

var type: NSPrinter.TypeName

A description of the printer’s make and model.

### Getting Page and Printer Information

func pageSize(forPaper: NSPrinter.PaperName) -> NSSize

Returns the size of the page for the specified paper type.

struct PaperName

The type you use to specify the name of a type of paper.

var languageLevel: Int

The PostScript language level recognized by the printer.

### Querying Tables

var deviceDescription: [NSDeviceDescriptionKey : Any]

A dictionary of keys and values that describe the device.

### Deprecated

enum TableStatus

Constants that describe the state of a printer information table stored by a printer object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Print Information

class NSPrintInfo

An object that stores information that’s used to generate printed output.

class NSPrintOperation

An object that controls operations that generate Encapsulated PostScript (EPS) code, Portable Document Format (PDF) code, or print jobs.

