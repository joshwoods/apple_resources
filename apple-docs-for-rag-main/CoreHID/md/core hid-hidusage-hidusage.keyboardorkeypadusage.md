

- Core HID
- HIDUsage
-  HIDUsage.KeyboardOrKeypadUsage 

Enumeration

# HIDUsage.KeyboardOrKeypadUsage

macOS 15.0+

``` source
enum KeyboardOrKeypadUsage
```

## Topics

### Enumeration Cases

case currencySubUnit

case currencyUnit

case decimalSeparator

case errorRollOver

case errorUndefined

case keyboard0AndRightBracket

case keyboard1AndBang

case keyboard2AndAt

case keyboard3AndHash

case keyboard4AndDollar

case keyboard5AndPercent

case keyboard6AndCaret

case keyboard7AndAmpersand

case keyboard8AndStar

case keyboard9AndLeftBracket

case keyboardA

case keyboardAgain

case keyboardAlternateErase

case keyboardApplication

case keyboardB

case keyboardBackslashAndPipe

case keyboardC

case keyboardCancel

case keyboardCapsLock

case keyboardClear

case keyboardClearAgain

case keyboardCommaAndLessThan

case keyboardCopy

case keyboardCrSelProps

case keyboardCut

case keyboardD

case keyboardDashAndUnderscore

case keyboardDelete

case keyboardDeleteForward

case keyboardDownArrow

case keyboardE

case keyboardEnd

case keyboardEqualsAndPlus

case keyboardEscape

case keyboardExSel

case keyboardExecute

case keyboardF

case keyboardF1

case keyboardF10

case keyboardF11

case keyboardF12

case keyboardF13

case keyboardF14

case keyboardF15

case keyboardF16

case keyboardF17

case keyboardF18

case keyboardF19

case keyboardF2

case keyboardF20

case keyboardF21

case keyboardF22

case keyboardF23

case keyboardF24

case keyboardF3

case keyboardF4

case keyboardF5

case keyboardF6

case keyboardF7

case keyboardF8

case keyboardF9

case keyboardFind

case keyboardForwardSlashAndQuestionMark

case keyboardG

case keyboardGraveAccentAndTilde

case keyboardH

case keyboardHelp

case keyboardHome

case keyboardI

case keyboardInsert

case keyboardInternational1

case keyboardInternational2

case keyboardInternational3

case keyboardInternational4

case keyboardInternational5

case keyboardInternational6

case keyboardInternational7

case keyboardInternational8

case keyboardInternational9

case keyboardJ

case keyboardK

case keyboardL

case keyboardLANG1

case keyboardLANG2

case keyboardLANG3

case keyboardLANG4

case keyboardLANG5

case keyboardLANG6

case keyboardLANG7

case keyboardLANG8

case keyboardLANG9

case keyboardLeftAlt

case keyboardLeftAposAndDouble

case keyboardLeftArrow

case keyboardLeftBrace

case keyboardLeftControl

case keyboardLeftGUI

case keyboardLeftShift

case keyboardLockingCapsLock

case keyboardLockingNumLock

case keyboardLockingScrollLock

case keyboardM

case keyboardMenu

case keyboardMute

case keyboardN

case keyboardNonUSBackslashAndPipe

case keyboardNonUSHashAndTilde

case keyboardO

case keyboardOper

case keyboardOut

case keyboardP

case keyboardPageDown

case keyboardPageUp

case keyboardPaste

case keyboardPause

case keyboardPeriodAndGreaterThan

case keyboardPower

case keyboardPrintScreen

case keyboardPrior

case keyboardQ

case keyboardR

case keyboardReturn

case keyboardReturnEnter

case keyboardRightAlt

case keyboardRightArrow

case keyboardRightBrace

case keyboardRightControl

case keyboardRightGUI

case keyboardRightShift

case keyboardS

case keyboardScrollLock

case keyboardSelect

case keyboardSemiColonAndColon

case keyboardSeparator

case keyboardSpacebar

case keyboardStop

case keyboardSysReqAttention

case keyboardT

case keyboardTab

case keyboardU

case keyboardUndo

case keyboardUpArrow

case keyboardV

case keyboardVolumeDown

case keyboardVolumeUp

case keyboardW

case keyboardX

case keyboardY

case keyboardZ

case keypad0AndInsert

case keypad1AndEnd

case keypad2AndDownArrow

case keypad3AndPageDn

case keypad4AndLeftArrow

case keypad5

case keypad6AndRightArrow

case keypad7AndHome

case keypad8AndUpArrow

case keypad9AndPageUp

case keypadA

case keypadAmpersand

case keypadAt

case keypadB

case keypadBackspace

case keypadBang

case keypadBar

case keypadBinary

case keypadC

case keypadCaret

case keypadClear

case keypadClearEntry

case keypadColon

case keypadComma

case keypadD

case keypadDash

case keypadDecimal

case keypadDouble0

case keypadDoubleAmpersand

case keypadDoubleBar

case keypadE

case keypadENTER

case keypadEqualSign

case keypadEquals

case keypadF

case keypadForwardSlash

case keypadGreater

case keypadHash

case keypadHexadecimal

case keypadLeftBrace

case keypadLeftBracket

case keypadLess

case keypadMemoryAdd

case keypadMemoryClear

case keypadMemoryDivide

case keypadMemoryMultiply

case keypadMemoryRecall

case keypadMemoryStore

case keypadMemorySubtract

case keypadNumLockAndClear

case keypadOctal

case keypadPercentage

case keypadPeriodAndDelete

case keypadPlus

case keypadPlusMinus

case keypadRightBrace

case keypadRightBracket

case keypadSpace

case keypadStar

case keypadTab

case keypadTriple0

case keypadXOR

case postFail

case thousandsSeparator

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

