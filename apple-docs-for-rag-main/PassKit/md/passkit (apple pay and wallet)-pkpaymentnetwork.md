

- PassKit (Apple Pay and Wallet)
-  PKPaymentNetwork 

Structure

# PKPaymentNetwork

A type that represents a payment method.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct PKPaymentNetwork
```

## Topics

### Payment networks

static let amex: PKPaymentNetwork

An American Express payment card.

static let bancomat: PKPaymentNetwork

A Bancomat payment card.

Deprecated

static let bancontact: PKPaymentNetwork

A Bancontact payment card.

static let bankAxept: PKPaymentNetwork

static let barcode: PKPaymentNetwork

A QR code to use for payment.

static let carteBancaire: PKPaymentNetworkDeprecated

static let cartesBancaires: PKPaymentNetwork

A Cartes Bancaires payment card.

static let chinaUnionPay: PKPaymentNetwork

A China Union Pay payment card.

static let dankort: PKPaymentNetwork

The Dankort payment card.

static let discover: PKPaymentNetwork

A Discover payment card.

static let eftpos: PKPaymentNetwork

The electronic funds transfer at point of sale (EFTPOS) payment method.

static let electron: PKPaymentNetwork

An Electron debit card.

static let elo: PKPaymentNetwork

The Elo payment card.

static let girocard: PKPaymentNetwork

A Girocard payment method.

static let idCredit: PKPaymentNetwork

An iD payment card.

static let interac: PKPaymentNetwork

The Interac payment method.

static let JCB: PKPaymentNetwork

A JCB payment card.

static let mada: PKPaymentNetwork

A mada payment card.

static let maestro: PKPaymentNetwork

A Maestro payment card.

static let masterCard: PKPaymentNetwork

A Mastercard payment card.

static let meeza: PKPaymentNetwork

static let mir: PKPaymentNetwork

A Mir payment card.

static let nanaco: PKPaymentNetwork

A Nanaco payment card.

static let NAPAS: PKPaymentNetwork

static let pagoBancomat: PKPaymentNetwork

static let postFinance: PKPaymentNetwork

A PostFinance AG payment card.

static let privateLabel: PKPaymentNetwork

Store credit and debit cards.

static let quicPay: PKPaymentNetwork

A QUICPay payment card.

static let suica: PKPaymentNetwork

A Suica payment card.

static let tmoney: PKPaymentNetwork

The TMoney card.

static let visa: PKPaymentNetwork

A Visa payment card.

static let vPay: PKPaymentNetwork

A Visa V Pay payment card.

static let waon: PKPaymentNetwork

A WAON payment card.

static let carteBancaires: PKPaymentNetwork

A Cartes Bancaires payment card.

Deprecated

### Initializers

init(String)

Creates a new payment network structure with the raw value you provide.

init(rawValue: String)

Creates a new payment network structure with the string you provide.

### Type Properties

static let himyan: PKPaymentNetwork

static let jaywan: PKPaymentNetwork

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Selecting the payment networks

class func availableNetworks() -> [PKPaymentNetwork]

Returns the list of available payment methods that Apple Pay supports.

var supportedNetworks: [PKPaymentNetwork]

The payment methods that you support.

