

- Foundation
-  NSCopying 

Protocol

# NSCopying

A protocol that objects adopt to provide functional copies of themselves.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSCopying
```

## Overview

The exact meaning of “copy” can vary from class to class, but a copy must be a functionally independent object with values identical to the original at the time the copy was made. A copy produced with NSCopying is implicitly retained by the sender, who is responsible for releasing it.

NSCopying declares one method, copy(with:), but copying is commonly invoked with the convenience method copy(). The copy() method is defined for all objects inheriting from NSObject and simply invokes copy(with:) with the default zone.

Your options for implementing this protocol are as follows:

- Implement NSCopying using alloc and `init...` in classes that don’t inherit copy(with:).

- Implement NSCopying by invoking the superclass’s copy(with:) when `NSCopying` behavior is inherited. If the superclass implementation might use the NSCopyObject function, make explicit assignments to pointer instance variables for retained objects.

- Implement NSCopying by retaining the original instead of creating a new copy when the class and its contents are immutable.

If a subclass inherits NSCopying from its superclass and declares additional instance variables, the subclass has to override copy(with:) to properly handle its own instance variables, invoking the superclass’s implementation first.

## Topics

### Copying

func copy(with: NSZone?) -> Any

Returns a new instance that’s a copy of the receiver.

**Required**

## Relationships

### Conforming Types

- ByteCountFormatter
- CachedURLResponse
- DateComponentsFormatter
- DateFormatter
- DateIntervalFormatter
- Dimension
- EnergyFormatter
- Formatter
- HTTPURLResponse
- ISO8601DateFormatter
- LengthFormatter
- ListFormatter
- MassFormatter
- MeasurementFormatter
- MessagePort
- NSAffineTransform
- NSAppleEventDescriptor
- NSAppleScript
- NSArray
- NSAttributedString
- NSCalendar
- NSCharacterSet
- NSComparisonPredicate
- NSCompoundPredicate
- NSCountedSet
- NSData
- NSDataDetector
- NSDate
- NSDateComponents
- NSDateInterval
- NSDecimalNumber
- NSDictionary
- NSError
- NSException
- NSExpression
- NSExtensionItem
- NSFileSecurity
- NSHashTable
- NSIndexPath
- NSIndexSet
- NSItemProvider
- NSLocale
- NSMachPort
- NSMapTable
- NSMeasurement
- NSMutableArray
- NSMutableAttributedString
- NSMutableCharacterSet
- NSMutableData
- NSMutableDictionary
- NSMutableIndexSet
- NSMutableOrderedSet
- NSMutableSet
- NSMutableString
- NSMutableURLRequest
- NSNotification
- NSNull
- NSNumber
- NSOrderedSet
- NSOrthography
- NSPersonNameComponents
- NSPointerArray
- NSPointerFunctions
- NSPredicate
- NSPurgeableData
- NSRegularExpression
- NSSet
- NSSortDescriptor
- NSString
- NSTextCheckingResult
- NSTimeZone
- NSURL
- NSURLComponents
- NSURLQueryItem
- NSURLRequest
- NSUUID
- NSUserNotification
- NSUserNotificationAction
- NSValue
- NumberFormatter
- PersonNameComponentsFormatter
- Port
- RelativeDateTimeFormatter
- Scanner
- SocketPort
- URLCredential
- URLProtectionSpace
- URLResponse
- URLSessionConfiguration
- URLSessionDataTask
- URLSessionDownloadTask
- URLSessionStreamTask
- URLSessionTask
- URLSessionUploadTask
- URLSessionWebSocketTask
- Unit
- UnitAcceleration
- UnitAngle
- UnitArea
- UnitConcentrationMass
- UnitDispersion
- UnitDuration
- UnitElectricCharge
- UnitElectricCurrent
- UnitElectricPotentialDifference
- UnitElectricResistance
- UnitEnergy
- UnitFrequency
- UnitFuelEfficiency
- UnitIlluminance
- UnitInformationStorage
- UnitLength
- UnitMass
- UnitPower
- UnitPressure
- UnitSpeed
- UnitTemperature
- UnitVolume
- XMLDTD
- XMLDTDNode
- XMLDocument
- XMLElement
- XMLNode

## See Also

### Copying

protocol NSMutableCopying

A protocol that mutable objects adopt to provide functional copies of themselves.

