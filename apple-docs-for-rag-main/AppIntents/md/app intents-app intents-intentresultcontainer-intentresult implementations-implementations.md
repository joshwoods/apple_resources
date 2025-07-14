

- App Intents
- App intents
- IntentResultContainer
-  IntentResult Implementations 

API Collection

# IntentResult Implementations

## Topics

### Type Methods

static func result() -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Intent>(actionButtonIntent: Intent) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Intent>(actionButtonIntent: Intent, activityIdentifier: String) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Intent>(actionButtonIntent: Intent, activityIdentifier: String, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Intent>(actionButtonIntent: Intent, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result(dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;OpensAppIntent>(opensIntent: OpensAppIntent) -> Self

Indicates the `AppIntent` finished performing

static func result(opensIntent: some AppIntent) -> Self

Indicates the `AppIntent` finished performing

static func result(opensIntent: some AppIntent, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;OpensAppIntent>(opensIntent: OpensAppIntent, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value>(value: Value) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent, activityIdentifier: String) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent, activityIdentifier: String, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value, Intent>(value: Value, actionButtonIntent: Intent, dialog: IntentDialog) -> Self

Indicates the Intent finished performing with an `AppIntent` to continue with

static func result&lt;Value>(value: Value, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value>(value: Value, opensIntent: some AppIntent) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, OpensAppIntent>(value: Value, opensIntent: OpensAppIntent) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value>(value: Value, opensIntent: some AppIntent, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

static func result&lt;Value, OpensAppIntent>(value: Value, opensIntent: OpensAppIntent, dialog: IntentDialog) -> Self

Indicates the `AppIntent` finished performing

