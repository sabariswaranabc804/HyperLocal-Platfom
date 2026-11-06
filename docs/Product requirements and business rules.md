# Location-Based Multi-Industry Marketplace Platform

**Product Requirements Document (PRD)**  
**Version:** 1.0  
**Status:** Product scope confirmed – technical decisions pending

---

## 1. Product Overview

Build a location-based, configurable, multi-industry marketplace connecting customers with nearby shops, businesses and service providers.

The platform initially supports three industries:

1. Grocery
2. Laundry
3. Home Services

Customers can discover businesses, compare products and services, place orders, book services, pay online or in cash, and track order or service progress.

The platform must support multiple cities and allow the Super Admin to add future industries, categories, forms, workflows and business rules through configuration wherever practical.

## 2. Product Applications

The platform consists of four applications.

| Application | Main users | Purpose |
|---|---|---|
| Customer App | Customers and guests | Discover, order, book, pay and track |
| Business App | Owners, managers and staff | Manage businesses, orders, bookings and operations |
| Agent App | Delivery agents and technicians | Accept assignments and update progress |
| Super Admin Web | Platform Super Admin | Manage the entire platform |

All four applications launch together.

### Development design order

1. Super Admin Web
2. Business App
3. Customer App
4. Agent App

## 3. MVP Scope

All three industries and all four applications are included in the MVP.

### Customer App

- Guest browsing and search.
- Mobile OTP authentication.
- GPS and manual location selection.
- Saved customer addresses.
- Nearby business discovery.
- Global product and service search.
- Category browsing and filters.
- Product comparison across nearby shops.
- Grocery cart and checkout.
- Laundry booking.
- Home service booking.
- Online payment and cash payment.
- Order and booking history.
- Order and service status tracking.
- Live GPS tracking when an agent is assigned and sharing location.
- Ratings and reviews after eligible completed transactions.
- English and Tamil.
- Light and dark themes.

### Business App

- Business registration and verification.
- Independent business and organization registration.
- Multi-branch management.
- Business profile and branding.
- Product and service catalogue.
- Pricing and availability management.
- Order and booking management.
- Automatic or manual order confirmation.
- Staff accounts and role-based permissions.
- Delivery agent and technician assignment.
- Business schedules and temporary closures.
- Payment and settlement information.
- Subscription management.
- Reports and activity logs.

### Agent App

- Independent agent registration.
- Business-added agent registration.
- Identity and document verification.
- Online/offline availability.
- Scheduled working hours.
- Assignment notifications.
- Accept or reject assignments according to configured rules.
- Pickup, delivery and service status updates.
- GPS location sharing when required.
- Assignment history.
- Earnings/payment information recorded by the platform.

### Super Admin Web

- Executive dashboard and operational dashboard.
- Industry management.
- Category management.
- Dynamic Form Builder.
- Workflow Builder.
- Business and organization management.
- Branch management.
- Business verification.
- Customer management.
- Agent and technician management.
- City and area management.
- Commission configuration.
- Subscription plans.
- Payment and settlement monitoring.
- GST configuration and reports.
- Promotions and coupons.
- Notification management.
- Customer support and complaint escalation.
- Analytics and reports.
- Platform settings.
- Security, privacy and audit management.

## 4. Industry Management

The Super Admin can create and manage industries dynamically.

Initial industries:

- Grocery
- Laundry
- Home Services

Industry configuration includes:

- Name, description, icon and image.
- English and Tamil translations.
- Categories and subcategories.
- Business registration requirements.
- Custom forms and fields.
- Product or service attributes.
- Pricing rules.
- Commissions.
- Payment methods.
- Delivery charges.
- Workflows and statuses.
- Notification templates.
- Business rules.
- Availability rules.

### Industry activation

Before activation, validate:

- Industry information.
- Categories.
- Required forms.
- Customer-facing screens.
- Workflows.
- Pricing and commission.
- Payment methods.
- Notification rules.
- Business registration requirements.
- Preview and configuration completeness.

### Configuration versioning

Support published versions, editable drafts, change history, comparison and rollback.

Safe changes can be applied immediately. Critical changes must use a draft, validation, impact review and publish process.

Existing transactions must retain their applicable historical configuration.

## 5. Category Management

- Configurable category depth by industry.
- Reusable master category templates.
- Industry-specific category customization.
- English and Tamil names and descriptions.
- Category images.
- Manual drag-and-drop ordering.
- Optional alphabetical or popularity sorting.

## 6. Dynamic Form Builder

The platform must support configurable forms without requiring code changes for ordinary form configuration.

### Field types

- Text and number.
- Email.
- Dropdown.
- Radio and checkbox.
- Date and time.
- Image and file upload.
- Conditional fields.
- Repeatable sections.
- Reusable field groups.

### Layouts

- Single column.
- Two columns.
- Grouped sections.
- Tabs.
- Multi-step forms.
- Responsive layouts.

### Form assignment

Forms can be assigned to:

- Industries.
- Categories.
- Businesses.
- Branches.
- Customers.
- Agents and technicians.
- Other supported user types.

### Submission management

- Pending, approved, rejected and returned statuses.
- Comments and attachments.
- Submission history.
- Resubmission.
- Search and filters.
- Role-based access.

Platform-required fields cannot be overridden by businesses.

## 7. Workflow Builder

Support both simple configuration and visual drag-and-drop workflow creation.

### Workflow capabilities

- Status creation and ordering.
- Status transitions.
- Conditions.
- Actions.
- Approval steps.
- Manual updates.
- Automatic updates.
- Cancellation rules.
- Notifications.

### Initial workflow templates

- Grocery order.
- Delivery.
- Laundry pickup and delivery.
- Home service booking.
- Inspection and quotation.
- Cancellation and refund.
- Business verification.
- Catalogue approval.

### Workflow migration

When a workflow changes, allow:

1. New transactions only.
2. Selected existing transactions.
3. All eligible existing transactions after impact review.

Preview, compatibility checks and confirmation are required before migration.

Use predefined safe action types and controlled execution rather than arbitrary code execution.

## 8. Business and Organization Management

Support two business structures:

- Independent single-location business.
- Organization with multiple branches.

### Registration and verification

- Common basic registration form.
- Industry-specific dynamic form.
- Owner identity proof.
- Business registration or proof.
- Address proof.
- Basic business information.
- Manual Super Admin approval.

Verification renewal periods and requirements must be configurable.

### Branch management

Organization owners can add branches. Super Admin controls automatic or manual branch approval.

Each branch can have its own:

- Address and service area.
- Business hours.
- Staff.
- Products and services.
- Pricing.
- Availability.
- Operational settings.

## 9. Catalogue and Availability

### Grocery

- Product name and description.
- Brand.
- Weight and unit.
- Variants.
- Images.
- Selling price.
- Availability.

### Laundry

- Garment type.
- Washing type.
- Quantity.
- Service price.
- Pickup and delivery details.
- Availability.

### Home Services

- Service type.
- Duration.
- Required skills.
- Inspection requirement.
- Fixed price or quotation.
- Service availability.

### Catalogue model

- Super Admin maintains a shared master catalogue.
- Businesses can use master items or create custom items.
- Approval rules are configurable by industry, category, business and item type.
- Minor changes can be immediate.
- Important changes can require approval.

**Inventory management is explicitly excluded from MVP.**

No stock quantity, warehouse management, inventory accounting or automatic stock deduction. Businesses manually mark items available or unavailable.

## 10. Location and Discovery

Support multiple cities at launch.

Super Admin manages:

- Cities.
- Areas and localities.
- Postal codes.
- Serviceability.
- Configurable radius.
- Industry availability.
- Business coverage.

Customers can use GPS, manually enter an address, select a map pin or choose a saved address.

### Search and ranking

Support:

- Category browsing.
- Global product and service search.
- Distance filters.
- Price filters.
- Rating filters.
- Availability filters.
- Product comparison across nearby shops.

Ranking can use distance, relevance, ratings, availability and business performance, with configurable weights.

## 11. Ordering and Booking

### Grocery

- Single-shop cart for MVP.
- Customer places an order.
- Business can automatically or manually confirm.
- Unavailable items can be rejected or replaced with customer approval.
- Customer and business cancellation rules.
- Order status history.

### Laundry

- Service selection.
- Quantity and garment details.
- Pickup and delivery scheduling.
- Booking status management.
- Assignment and completion confirmation.

### Home Services

- Service selection and booking.
- Technician assignment.
- Inspection where required.
- Quotation generation.
- Customer approval before additional work.
- Revised quotations for scope changes.
- Service completion.
- Customer confirmation or issue reporting within a configurable period.

### Cart limitation

MVP supports one shop per order. Architecture should permit future multi-shop checkout and split orders.

## 12. Delivery and Agent Management

### Agent onboarding

Support independent self-registration and business-added agents, with verification.

### Assignment

Hybrid assignment model:

- Business manual assignment.
- Platform recommendations.
- Automatic assignment.

Assignment suggestions can consider distance and agent availability.

If an agent does not accept an assignment:

- Retry after a configurable interval.
- Offer to another eligible agent.
- Notify the business.
- Allow manual reassignment after the retry limit.

### Availability

- Online/offline toggle.
- Scheduled working days.
- Working hours.
- Temporary pause.

### Agent payments

The business pays the delivery agent directly under the initial model. The platform records assignment and payment information.

Rules for platform agents serving multiple businesses must be validated before launch.

### Tracking

- Status timeline.
- Live GPS when an agent is assigned and sharing location.
- ETA where reliable location and routing data are available.
- Configurable location update frequency.

## 13. Service Provider Management

Support independent service providers and service organizations.

Organizations can manually assign technicians or enable automatic assignment.

Assignment can consider:

- Skills.
- Location.
- Availability.
- Workload.

Organization admins can reassign technicians.

Independent providers manage their own bookings.

## 14. Payments, Commissions and Settlements

### Payment methods

- UPI.
- Cards.
- Net banking.
- Cash on delivery.
- Cash after service.

### Payment collection

Configurable by industry and business:

- Direct business settlement.
- Platform collects and settles with business.

### Commission

Configurable by:

- Industry.
- Business.
- Category.
- Transaction type.

Support subscription revenue and transaction commission.

### Delivery charges

Hybrid configurable pricing:

- Fixed charge.
- Distance-based charge.
- Minimum charge.
- Free delivery thresholds.
- Industry-specific and business-specific rules.

### Refunds

Hybrid model:

- Automatic refunds for predefined eligible cases.
- Business review for other refund requests.
- Super Admin monitoring and platform-level dispute intervention.

Record refund reason, amount, status and transaction history.

Actual refund execution must follow gateway and settlement permissions.

### Settlement schedules

Configurable by Super Admin:

- Daily.
- Weekly.
- Monthly.
- Business-specific schedule.
- Minimum payout amount.
- Hold period.
- Pending balance.
- Failed settlement handling.

### GST

Hybrid configurable GST management:

- Rules by industry, business and transaction type.
- Applicable tax rates.
- Tax-inclusive and tax-exclusive pricing.
- Appropriate invoices and reports.
- Separate product, service, delivery and commission tax records.
- Historical tax records for auditing.

Tax treatment must be validated by a qualified CA against applicable Indian GST requirements.

## 15. Subscription Management

Support configurable monthly and yearly plans.

Plan settings:

- Pricing.
- Features.
- Industry eligibility.
- Business-size eligibility.
- Branch limits.
- Staff limits.
- Service limits.
- Trial period.
- Upgrade and downgrade.
- Renewal and expiry.

### Expiry handling

Configurable:

- Grace period.
- Read-only mode.
- Restriction on new orders or bookings.
- Suspension.
- Reactivation.

## 16. Customer Support and Complaints

Hybrid support model:

- Basic support and complaint submission in MVP.
- Business handles normal complaints.
- Customers can escalate unresolved issues.
- Fraud, safety and payment disputes can be escalated to Super Admin.

Support ticket and chat capabilities can expand by industry and business.

Maintain complaint status, messages, evidence and resolution history.

## 17. Ratings and Reviews

Eligible completed transactions can receive ratings for:

- Business.
- Products.
- Services.
- Delivery agents.

Prevent ratings for transactions that have not reached the required completion status.

## 18. Promotions and Coupons

Hybrid model:

- Super Admin platform campaigns.
- Business-created offers.

Support fixed and percentage discounts, validity periods, eligibility rules and usage analytics.

## 19. Notifications

Channels:

- Push notifications.
- SMS.
- WhatsApp.
- Email.

Super Admin manages global templates and rules. Businesses can customize permitted messages and settings.

OTP and payment confirmation messages remain platform-controlled.

Customer notification preferences must be respected where applicable.

## 20. Staff and Permissions

Advanced role-based access control.

Support:

- Predefined roles.
- Custom roles.
- Granular permissions.
- Branch-level access.
- Activity logs.

Example roles:

- Owner.
- Manager.
- Cashier.
- Order Handler.
- Delivery Coordinator.
- Technician.

## 21. Dashboards and Analytics

### Super Admin dashboard

Hybrid executive and operational dashboard.

- Revenue and transaction overview.
- Industry performance.
- City performance.
- Business onboarding and verification.
- Active customers.
- Orders and bookings.
- Payment and settlement monitoring.
- Subscription status.
- Complaints and operational tasks.

Dashboard widgets can be shown, hidden, rearranged and filtered by date, industry and city. Save preferences and support reset.

### Business reports

- Orders.
- Bookings.
- Revenue.
- Customer activity.
- Service performance.
- Delivery performance.
- Payment summaries.

### Customer analytics

- Total, active and new customers.
- Location distribution.
- Industry preferences.
- Order and booking history.
- Retention.
- Segmentation.
- Lifetime value.
- Configurable reports.

## 22. Languages, Branding and UI

### Languages

English and Tamil in MVP.

- Detect device language.
- Fall back to English for unsupported languages.
- Allow manual language selection.
- Save user preference.

### Branding

- Central platform identity.
- Business logos, banners and images.
- Business brand colours.
- Organization-level branding.
- Branch-specific information.

### Design system

- One shared design system across all four applications.
- Enterprise + Premium visual style.
- Light and dark modes.
- Responsive desktop, laptop, tablet and mobile layouts.
- Google Stitch prototypes before Antigravity implementation.

## 23. Security and Privacy

- Mobile OTP authentication for customers.
- Role-based authentication for business and platform users.
- Optional 2FA.
- Device and session management.
- Login logs.
- Logout from all devices.
- Consent management for location, notifications, personal data and marketing.
- Data access, export and deletion request handling.
- Consent history and audit logs.

Protect identity documents, location data, payment information and personal information.

## 24. Data Retention and Recovery

Configurable retention rules.

- Business data export.
- Historical order, booking and payment retention.
- Secure account closure.
- Deletion according to applicable legal requirements.
- Audit history.
- Scheduled backups.
- Point-in-time recovery where supported.
- Monitoring and restore testing.
- Defined recovery objectives (RPO/RTO).

## 25. Deployment and Engineering Requirements

Target a modular cloud deployment with containerization where appropriate.

Required environments:

- Development.
- Staging.
- Production.

Include:

- CI/CD pipelines.
- Monitoring and alerting.
- Centralized logs.
- Error tracking.
- Secure configuration and secrets management.
- Database backup and recovery.
- Scalable architecture.
- API documentation.
- Automated testing.

**Technology stack, database and cloud provider are not yet selected.** These must be evaluated after the PRD is approved.

## 26. Phase Planning

### MVP – First Release

- All four applications.
- Grocery, Laundry and Home Services.
- Multiple cities.
- Customer discovery, ordering and booking.
- Business onboarding and branch management.
- Agent and technician assignments.
- Payment and settlement support.
- Dynamic industry/category management.
- Dynamic Form Builder.
- Workflow Builder.
- Basic support and complaint escalation.
- English and Tamil.
- Light and dark themes.
- Reports, roles and audit logs.

### Phase 2

- Advanced recommendations.
- Loyalty and rewards.
- Advanced business intelligence.
- Advanced analytics.
- More sophisticated settlement automation.
- Fraud monitoring.
- Route optimization.
- Expanded live chat and support.
- Advanced workflow automation.

### Future

- Multi-shop checkout and split orders.
- Supplier and procurement management.
- Advanced fleet and logistics.
- Full accounting and ERP.
- AI-powered recommendations.
- Additional industries and languages.

## 27. Important Business Rules

1. One customer order belongs to one shop in MVP.
2. Inventory and warehouse management are excluded.
3. Only eligible completed transactions can receive ratings.
4. Customer OTP is required before order or booking confirmation.
5. Business approval and verification rules are configurable.
6. Existing transactions retain historical configuration versions.
7. Workflow migration requires compatibility and impact review.
8. Additional service work requires customer approval of the quotation.
9. Live tracking is available only when location sharing is active.
10. Payment, refund and settlement execution must respect gateway capabilities and applicable regulations.
11. Businesses handle normal complaints; serious and unresolved complaints have an escalation path.
12. Platform-required form fields and security rules cannot be overridden by businesses.

## 28. Open Decisions and Risks

The following require validation before implementation:

- Payment gateway and merchant settlement capabilities.
- GST treatment and invoicing requirements.
- Business and agent verification standards.
- Rules for agents working across multiple businesses.
- Customer complaint escalation and response times.
- Location tracking permissions and data retention.
- Subscription, commission and tax interactions.
- Data protection and applicable Indian legal requirements.
- Feasibility and implementation stages for no-code workflow and form builders.

## 29. Product Acceptance Criteria

The MVP is ready for release when:

- All three industries can be configured and operated.
- Customers can complete grocery orders and laundry/home-service bookings.
- Businesses can manage branches, staff and transactions.
- Agents can receive and update assignments.
- Super Admin can manage industries, categories, forms and workflows.
- Payment and settlement records are auditable.
- Customer support and complaint escalation work.
- English and Tamil interfaces are usable.
- Light and dark themes work across supported screen sizes.
- Role-based permissions are enforced.
- Critical flows pass functional, security and integration testing.
- Backup and recovery procedures have been tested.

---

**Document status:** Product scope consolidated.  
**Next stage:** Review and approve PRD → select technology stack → define architecture and database → create Google Stitch prototypes → implement through Antigravity.