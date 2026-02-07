## Solution Architecture

The solution is designed using a layered architecture approach to clearly
separate CRM, pricing intelligence, and commercial outputs.

### CRM Layer
Sales Cloud is used to manage Accounts, Contacts, and Opportunities.
Opportunities act as the entry point for the CPQ process.

### CPQ Engine Layer
Salesforce CPQ is responsible for:
- Product bundling and configuration
- Pricing calculation
- Volume-based discounting
- Enforcement of business rules
- Approval-driven discount governance

### Commercial Output Layer
Approved quotes are converted into:
- Contracts for agreement tracking
- Orders for fulfillment readiness

### Automation Strategy
The solution prioritizes Salesforce CPQ native capabilities such as
Product Rules and Price Rules. Apex is avoided unless CPQ limitations
require custom logic.
