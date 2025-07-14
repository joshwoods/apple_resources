

- Core HID
- HIDUsage
-  HIDUsage.BarcodeScannerUsage 

Enumeration

# HIDUsage.BarcodeScannerUsage

macOS 15.0+

``` source
enum BarcodeScannerUsage
```

## Topics

### Enumeration Cases

case activeTime

case addEAN2Of3LabelDefinition

case aimDuration

case aimingLaserPattern

case aimingOrPointerMode

case attributeReport

case aztecCode

case barCodePresent

case barCodePresentSensor

case barCodeScannerCradle

case barSpaceData

case barcodeBadgeReader

case barcodeScanner

case bc412

case beeperState

case booklandEAN

case channelCode

case check

case checkDigit

case checkDigitCodabarEnable

case checkDigitCode39Enable

case checkDigitDisable

case checkDigitEnableInterleaved2Of5OPCC

case checkDigitEnableInterleaved2Of5USS

case checkDigitEnableOneMSIPlessey

case checkDigitEnableStandard2Of5OPCC

case checkDigitEnableStandard2Of5USS

case checkDigitEnableTwoMSIPlessey

case checkDisablePrice

case checkEnable4DigitPrice

case checkEnable5DigitPrice

case checkEnableEuropean4DigitPrice

case checkEnableEuropean5DigitPrice

case class1ALaser

case class2Laser

case clearAllEAN2Of3LabelDefinitions

case codabar

case codabarControlReport

case code128

case code128ControlReport

case code16

case code32

case code39

case code39ControlReport

case code49

case code93

case codeOne

case colorcode

case commitParametersToNVM

case constantElectronicArticleSurveillance

case contactScanner

case controlReport2D

case convertEAN8To13Type

case convertUPCAToEAN13

case convertUPCEToA

case cordlessScannerBase

case dataLengthMethod

case dataMatrix

case dataPrefix

case decodeDataContinued

case decodedData

case disableCheckDigitTransmit

case discreteLengthToDecode1

case discreteLengthToDecode2

case dlMethodCheckForDiscrete

case dlMethodCheckInRange

case dlMethodReadAny

case dumbBarCodeScanner

case ean13

case ean13FlagDigit1

case ean13FlagDigit2

case ean13FlagDigit3

case ean2Of3LabelControlReport

case ean8

case ean8FlagDigit1

case ean8FlagDigit2

case ean8FlagDigit3

case ean99128Mandatory

case ean99P5Or128Optional

case eanThreeLabel

case eanTwoLabel

case electronicArticleSurveillanceNotification

case enableCheckDigitTransmit

case enableEANTwoLabel

case errorIndication

case fixedBeeper

case fragmentDecoding

case fullASCIIConversion

case goodDecodeIndication

case goodReadLED

case goodReadLampDuration

case goodReadLampIntensity

case goodReadToneFrequency

case goodReadToneLength

case goodReadToneVolume

case goodReadWhenToWrite

case grwtiAfterDecode

case grwtiBeepOrLampAfterTransmit

case grwtiNoBeepOrLampUseAtAll

case handsFreeScanning

case heaterPresent

case initiateBarcodeRead

case interleaved2Of5

case interleaved2Of5ControlReport

case intrinsicallySafe

case italianPharmacyCode

case klasseEinsLaser

case laserOnTime

case laserState

case lockoutTime

case longRangeScanner

case maxiCode

case maximumLengthToDecode

case microPDF

case minimumLengthToDecode

case mirrorSpeedControl

case miscellaneous1DControlReport

case motorState

case motorTimeout

case msiOrPlessey

case msiPlesseyControlReport

case multiRangeScanner

case noReadMessage

case notOnFileIndication

case notOnFileVolume

case parameterScanning

case parametersChanged

case pdf417

case periodical

case periodicalAutoDiscriminatePlus2

case periodicalAutoDiscriminatePlus5

case periodicalIgnorePlus2

case periodicalIgnorePlus5

case periodicalOnlyDecodeWithPlus2

case periodicalOnlyDecodeWithPlus5

case polarityInvertedBarCode

case polarityNormalBarCode

case posiCode

case powerOnResetScanner

case powerupBeep

case prefixAIMI

case prefixNone

case prefixProprietary

case preventReadOfBarcodes

case programmableBeeper

case proximitySensor

case qrCode

case rawDataPolarity

case rawScannedDataReport

case scannedDataReport

case scannerDataAccuracy

case scannerInCradle

case scannerInRange

case scannerReadConfidence

case setParameterDefaultValues

case settingsReport

case soundErrorBeep

case soundGoodReadBeep

case soundNotOnFileBeep

case standard2Of5

case standard2Of5ControlReport

case standard2Of5IATA

case statusReport

case superCode

case symbologyIdentifier1

case symbologyIdentifier2

case symbologyIdentifier3

case transmitCheckDigit

case transmitStartOrStop

case triOptic

case triggerMode

case triggerModeBlinkingLaserOn

case triggerModeContinuousLaserOn

case triggerModeLaserOnWhilePulled

case triggerModeLaserStaysOnAfterRelease

case triggerReport

case triggerState

case triggerless

case uccOrEAN128

case ultraCode

case upcA

case upcAWith128Mandatory

case upcAWith128Optional

case upcAWithP5Optional

case upcE

case upcE1

case upcOrEAN

case upcOrEANControlReport

case upcOrEANCouponCode

case upcOrEANPeriodicals

case usd5SlugCode

case veriCode

case wand

case waterResistant

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

