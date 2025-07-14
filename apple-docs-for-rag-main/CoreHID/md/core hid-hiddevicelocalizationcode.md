

- Core HID
-  HIDDeviceLocalizationCode 

Enumeration

# HIDDeviceLocalizationCode

The localization codes that some HID devices declare to specify conformance to a certain format or language.

macOS 15.0+

``` source
enum HIDDeviceLocalizationCode
```

## Overview

This maps to the optional `bCountryCode` value in the HID descriptor.

For more details, see Human Interface Devices (HID) Specifications and Tools.

## Topics

### Operators

static func == (HIDDeviceLocalizationCode, HIDDeviceLocalizationCode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case arabic

This maps to Arabic in the HID specification.

case belgium

This maps to Belgian in the HID specification.

case canada

This maps to Canadian-bilingual in the HID specification.

case canadaFrench

This maps to Canadian-French in the HID specification.

case chineseZhuyin

This maps to Taiwan in the HID specification.

case czechia

This maps to Czech Republic in the HID specification.

case denmark

This maps to Danish in the HID specification.

case finland

This maps to Finnish in the HID specification.

case france

This maps to France in the HID specification.

case germany

This maps to German in the HID specification.

case greece

This maps to Greek in the HID specification.

case hebrew

This maps to Hebrew in the HID specification.

case hungary

This maps to Hungary in the HID specification.

case italy

This maps to Italian in the HID specification.

case japan

This maps to Japan (Katakana) in the HID specification.

case korea

This maps to Korean in the HID specification.

case latinAmerica

This maps to Latin America in the HID specification.

case netherlands

This maps to Netherlands/Dutch in the HID specification.

case norway

This maps to Norwegian in the HID specification.

case persian

This maps to Persian (Farsi) in the HID specification.

case poland

This maps to Poland in the HID specification.

case portugal

This maps to Portuguese in the HID specification.

case russia

This maps to Russia in the HID specification.

case slovakia

This maps to Slovakia in the HID specification.

case spain

This maps to Spanish in the HID specification.

case sweden

This maps to Swedish in the HID specification.

case switzerland

This maps to Switzerland in the HID specification.

case switzerlandFrench

This maps to Swiss/French in the HID specification.

case switzerlandGerman

This maps to Swiss/German in the HID specification.

case turkeyQWERTY

This maps to Turkish-Q in the HID specification.

case turkeyStandard

This maps to Turkish-F in the HID specification.

case unitedKingdom

This maps to UK in the HID specification.

case unitedStates

This maps to US in the HID specification.

case unitedStatesISO

This maps to International (ISO) in the HID specification.

case unsupported

This maps to Not Supported in the HID specification.

case yugoslavia

This maps to Yugoslavia in the HID specification.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Interaction

Communicating with human interface devices

Interact with and obtain data from devices such as keyboards and mice.

actor HIDDeviceClient

A client of a physical or virtual HID compatible peripheral.

struct HIDElement

A representation of an item from a report descriptor for a HID device.

struct HIDElementCollection

A collection of items from a report descriptor for a HID device.

struct Value

Data associated with a HID element.

protocol HIDElementUpdate

A base protocol for element update types.

enum HIDReportType

Types for HID reports.

struct HIDReportID

A type to represent the report IDs of HID reports.

enum HIDUsage

A type to represent HID usage pages.

enum HIDDeviceError

Errors that the framework can throw.

enum HIDDeviceTransport

Common transport types that transmit data to or from a HID device.

