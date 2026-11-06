# Product Requirements Document (PRD)

**Project:** Location-Based Multi-Industry Marketplace Platform  
**Version:** 0.1 – Product Discovery Draft  
**Status:** Initial Requirements Consolidation  
**Product Name:** To be decided  
**Technology Stack:** Not finalized

---

# 1. Product Overview

## 1.1 Product Concept

Build a configurable, location-based, multi-industry platform that connects customers with nearby shops, businesses and service providers.

Customers can discover nearby businesses, compare products and prices, purchase products, book services, arrange delivery and track their orders.

The platform initially targets:

1. Grocery
2. Laundry
3. Home Services

Additional industries can be introduced through Super Admin configuration.

## 1.2 Main Objective

Create one unified platform that supports multiple industries, business types, organizations, branches and service workflows without requiring a separate application for every industry.

## 1.3 Product Characteristics

- Location-based discovery.
- Multi-industry support.
- Dynamic industry configuration.
- Independent businesses and multi-branch organizations.
- Unified customer mobile application.
- Unified business and operations mobile application.
- Separate Super Admin web application.
- Configurable workflows and business rules.
- Subscription-based business model.
- Configurable transaction commissions.

# 2. Platform Applications

## 2.1 Customer Application

A unified mobile application for all supported industries.

Main features:
- Mobile OTP registration and login.
- Guest browsing.
- GPS and manual location selection.
- Saved addresses.
- Nearby business discovery.
- Industry and category browsing.
- Global product and service search.
- Product comparison across nearby shops.
- Product ordering.
- Service booking.
- Online and cash payments.
- Order and booking tracking.
- Live delivery tracking.
- Replacement approval.
- Cancellation and refund status.
- Ratings and reviews.
- English and Tamil languages.
- Push, SMS and WhatsApp notifications.

## 2.2 Business and Operations Application

One unified application with role-based workspaces.

Supported users:
- Business owner.
- Organization administrator.
- Branch manager.
- Staff.
- Order handler.
- Delivery coordinator.
- Delivery agent.
- Independent service provider.
- Technician.

Main features:
- Business registration.
- Document submission.
- Business profile management.
- Product catalogue management.
- Service catalogue management.
- Pricing management.
- Order management.
- Booking management.
- Customer communication.
- Delivery assignment.
- Technician assignment.
- Staff management.
- Business availability.
- Branch management.
- Business analytics.
- Subscription management.
- Payment and refund records.

## 2.3 Super Admin Web Application

A separate web application controlled by one platform owner (single Super Admin).

Main modules:
- Dashboard.
- Industry management.
- Category management.
- Dynamic form builder.
- Workflow builder.
- Business verification.
- Organization and branch management.
- City and area management.
- Subscription management.
- Commission management.
- Payment configuration.
- Delivery configuration.
- Notification configuration.
- Promotion management.
- Customer analytics.
- Business analytics.
- Platform settings.
- Security and audit logs.
- Data retention configuration.

# 3. Industry Management

## 3.1 Fully Dynamic Industry Configuration

Super Admin should be able to create and configure industries through the admin panel.

Configuration capabilities:

- Create, edit, activate and deactivate industries.
- Create industry-specific categories and subcategories.
- Configure product and service types.
- Configure custom fields.
- Configure forms.
- Configure workflow steps and statuses.
- Configure business rules.
- Configure industry-specific notifications.
- Configure pricing rules.
- Configure availability rules.
- Configure service areas.

The objective is to minimize developer involvement when introducing new industries.

## 3.2 Initial Industries

### Grocery
- Nearby grocery shops.
- Product catalogue.
- Product search across shops.
- Shop-specific pricing.
- Product ordering.
- Availability confirmation.
- Replacement suggestions.
- Delivery management.

### Laundry
- Nearby laundry businesses.
- Laundry service catalogue.
- Garment and wash-type selections.
- Service bookings.
- Pickup and delivery.
- Service status tracking.
- Pricing and quotation support where required.

### Home Services
- Electrician.
- Plumber.
- AC repair.
- Cleaning.
- Carpenter.
- Other configurable services.

Support direct bookings and quotation-based service requests.

# 4. Business and Organization Management

## 4.1 Supported Business Structures

Both structures must be supported:

**Independent business**
- One business owner.
- One business location.
- Independent business operations.

**Organization-based business**
- One organization.
- Multiple branches.
- Centralized organization management.
- Branch-level operations.
- Branch-level staff and permissions.
- Branch-level orders and reports.

## 4.2 Business Registration

Two registration methods:

- Business self-registration.
- Super Admin creates a business account.

All registrations require manual Super Admin approval.

## 4.3 Business Verification

Full verification is required:

- Owner identity proof.
- Business registration or business proof.
- Business address proof.
- Business contact details.

Super Admin reviews and approves or rejects applications.

Document renewal periods and requirements must be configurable.

# 5. Location and Discovery

## 5.1 Customer Location

Support:
- GPS detection.
- Manual address entry.
- Map-based location selection.
- Multiple saved addresses.
- Address selection for individual orders and bookings.

## 5.2 Business Location

Support:
- Multiple cities.
- Areas and localities.
- Postal codes.
- Business coverage mapping.
- Configurable serviceability.
- Industry availability by location.
- Configurable discovery and delivery radius.

## 5.3 Business Search Ranking

Configurable smart ranking based on:

- Distance.
- Ratings.
- Availability.
- Search relevance.
- Business performance.

## 5.4 Search

Customers can:
- Browse industries.
- Browse categories.
- Search products.
- Search services.
- Filter by distance.
- Filter by price.
- Filter by rating.
- Filter by availability.
- Compare product prices across nearby shops.

# 6. Product Catalogue and Pricing

## 6.1 Hybrid Catalogue

Super Admin maintains a master product catalogue.

Businesses can:
- Select products from the master catalogue.
- Add custom products.
- Edit descriptions and images.
- Set their own selling prices.

## 6.2 Inventory Exclusion

Inventory management is not included in the initial scope.

Specifically:
- No stock quantity management.
- No warehouse management.
- No inventory accounting.
- No automatic stock deduction.

Businesses can manually mark products as available or unavailable.

## 6.3 Pricing

Hybrid pricing:
- Super Admin can define suggested/default prices.
- Each business sets its own selling price.
- Shop-specific discounts and offers are supported.

# 7. Ordering and Availability

## 7.1 Order Acceptance

Each business can select:

- Automatic order acceptance.
- Manual order confirmation.

## 7.2 Unavailable Products

If an ordered item is unavailable:

1. Business identifies the unavailable item.
2. Business suggests a replacement or removes the item.
3. Customer receives a notification.
4. Customer approves or rejects the replacement.
5. Final order is updated accordingly.

## 7.3 Shopping Cart

Initial release:
- One shop per order.
- Customers can compare products across different shops.

Future:
- Multi-shop cart.
- Split orders.
- Separate delivery charges.
- Shop-wise order tracking.

## 7.4 Cancellation

Both customer and business can cancel orders according to order status and configured cancellation rules.

Cancellation reasons must be recorded.

# 8. Delivery Management

## 8.1 Delivery Methods

Support:
- Business-owned delivery agents.
- Platform-registered delivery agents.

## 8.2 Delivery Assignment

Hybrid assignment:

- Business manually assigns agents.
- Business selects available platform agents.
- Platform suggests or automatically assigns agents.
- Assignment considers location and availability.

## 8.3 Delivery Agent Registration

Both options:
- Independent agent registration.
- Business-created agent accounts.

Agent identity verification is required.

## 8.4 Agent Availability

Agents can:
- Switch Online/Offline.
- Configure working days.
- Configure working hours.
- Pause new assignments.

## 8.5 Delivery Payments

Business pays its delivery agents directly.

The platform records delivery assignments and relevant payment details.

## 8.6 Delivery Tracking

Customers can view:
- Order status timeline.
- Assigned agent details.
- Live GPS location.
- Estimated arrival time where available.
- Delivery completion confirmation.

# 9. Service Management

## 9.1 Provider Types

Support:
- Independent professionals.
- Service organizations.
- Organizations with multiple technicians.

## 9.2 Service Booking

Two booking methods:

**Direct booking**
- Customer selects a standard service.
- Selects date and time.
- Provider accepts.
- Service is performed.

**Quotation-based request**
- Customer describes the problem.
- Customer can attach images.
- Provider inspects the issue.
- Provider submits a quotation.
- Customer approves or rejects it.

## 9.3 Technician Assignment

Hybrid assignment:
- Organization admin manually assigns technicians.
- Automatic technician assignment is supported.
- Assignment considers skills, location and availability.
- Admin can reassign technicians.

Independent providers manage their own bookings.

## 9.4 Service Pricing

Support:
- Fixed service prices.
- Inspection-based quotations.
- Customer approval before additional work.
- Revised quotations when service scope changes.

## 9.5 Service Completion

1. Technician marks work completed.
2. Customer receives notification.
3. Customer confirms completion or raises an issue.
4. Configurable confirmation period applies.
5. Completion history is maintained.

# 10. Payments and Financial Management

## 10.1 Customer Payment Methods

Support:
- UPI.
- Cards.
- Net banking.
- Cash on delivery.
- Cash after service completion.

## 10.2 Payment Settlement

Configurable settlement models:

- Direct business settlement.
- Platform collection followed by business settlement.

Settlement configuration can vary by industry and business type.

## 10.3 Refunds

Business-controlled refund initiation.

Requirements:
- Refund amount.
- Refund reason.
- Refund transaction status.
- Customer notification.
- Refund history.

Payment gateway and settlement rules must determine the actual authorization and execution process.

## 10.4 Platform Revenue

Two revenue sources:

**Subscription**
- Monthly plans.
- Yearly plans.
- Configurable pricing.

**Transaction commission**
- Industry-specific rates.
- Business-specific rates.
- Category-specific rates.
- Transaction-type-specific rates.

# 11. Subscription Management

Super Admin can configure:

- Plan name.
- Monthly/yearly pricing.
- Features.
- Branch limits.
- Staff limits.
- Service limits.
- Industry-specific plans.
- Free trials.
- Upgrades and downgrades.
- Renewal and expiry.

## Subscription Expiry

Configurable rules:
- Grace period.
- Read-only access.
- Restrictions on accepting new orders/bookings.
- Automatic suspension.
- Reactivation after renewal.

# 12. Ratings and Reviews

Customers can separately rate:

- Business.
- Products.
- Services.
- Delivery agents.

Reviews are permitted only for eligible completed orders or bookings.

# 13. Customer Accounts and Guest Access

## Authentication
- Mobile OTP.
- No mandatory password.

## Guest Access

Customers can:
- Browse businesses.
- Search products and services.
- View prices and ratings.
- Add products to cart.
- Prepare bookings.

Login is required before confirming an order or booking.

# 14. Notifications

Supported channels:
- Push notifications.
- SMS.
- WhatsApp.
- Email.

Super Admin manages global templates and notification rules.

Businesses can customize permitted messages and preferences.

Templates support English and Tamil.

Important events include:
- OTP.
- Order placed.
- Order accepted/rejected.
- Replacement request.
- Delivery assignment.
- Delivery status.
- Booking confirmation.
- Technician assignment.
- Quotation approval.
- Payment.
- Refund.
- Subscription expiry.

# 15. Staff and Permissions

Advanced business staff management:

- Predefined roles.
- Custom roles.
- Granular permissions.
- Branch-level access.
- Staff activity logs.
- Configurable access policies.

Example roles:
- Owner.
- Manager.
- Cashier.
- Order Handler.
- Delivery Coordinator.
- Technician.

Super Admin remains a single account in the initial version.

# 16. Analytics and Reporting

## Business Reports

Detailed reports:
- Orders.
- Bookings.
- Revenue.
- Customer activity.
- Service performance.
- Delivery performance.
- Payment summaries.

## Super Admin Customer Analytics

Advanced analytics:
- Total customers.
- Active customers.
- New registrations.
- Customer locations.
- Industry preferences.
- Order and booking history.
- Retention.
- Customer segmentation.
- Customer lifetime value.
- Behaviour analytics.
- Configurable reports.

# 17. Promotions

Hybrid promotion management:

Super Admin:
- Platform-wide campaigns.
- Global coupons.
- Industry-specific promotions.

Businesses:
- Business-level offers.
- Product discounts.
- Service discounts.

Support:
- Fixed discounts.
- Percentage discounts.
- Coupon codes.
- Validity periods.
- Eligibility rules.
- Offer usage tracking.

# 18. Business Availability

Configurable schedules:

- Daily opening and closing hours.
- Multiple shifts.
- Break times.
- Weekly holidays.
- Special dates.
- Temporary closures.
- Branch-specific schedules.
- Service-specific availability.

# 19. Languages and Branding

## Languages

Initial languages:
- English.
- Tamil.

Architecture should permit additional languages later.

## Branding

Hybrid branding:
- One central platform identity.
- Business logos.
- Business banners.
- Business images.
- Business brand colours.
- Organization-level branding.
- Branch-specific details.

# 20. Privacy and Security

## Account Security

Support:
- Role-based authentication.
- Mobile OTP.
- Optional two-factor authentication.
- Device/session management.
- Login activity logs.
- Logout from all devices.

## Customer Privacy

Support:
- Consent management.
- Location permission.
- Notification permission.
- Marketing preferences.
- Data access requests.
- Data export.
- Account/data deletion requests.
- Consent history.
- Audit logs.

# 21. Data Management

Configurable data retention:

- Historical order retention.
- Historical booking retention.
- Payment record retention.
- Business data export.
- Business account closure.
- Data deletion according to applicable legal requirements.
- Audit history for important operations.

# 22. Backup and Recovery

Support:
- Configurable backup schedules.
- Point-in-time recovery.
- Backup monitoring.
- Disaster recovery procedures.
- Periodic restore testing.
- Defined Recovery Point Objective (RPO).
- Defined Recovery Time Objective (RTO).

# 23. Deployment and Infrastructure Requirements

Preferred deployment direction:

- Modular applications.
- Independent deployment where appropriate.
- Containerization where appropriate.
- CI/CD automation.
- Development environment.
- Staging environment.
- Production environment.
- Application monitoring.
- Infrastructure monitoring.
- Future scalability.

The actual cloud provider, backend architecture and database technology remain undecided.

# 24. Launch Strategy

## Initial Launch

Industries:
1. Grocery.
2. Laundry.
3. Home Services.

Geography:
- Multiple cities.

City management:
- Dynamic city creation.
- Areas and localities.
- Postal codes.
- Industry activation by location.
- Serviceability mapping.
- Configurable coverage radius.

## Future Expansion

The platform should allow:
- New industries.
- New categories.
- New business types.
- New service workflows.
- Additional languages.
- Multi-shop checkout.
- Supplier management.
- Additional integrations.

# 25. Initial Scope Exclusions

The following are not part of the initial scope unless later approved:

- Inventory and warehouse management.
- Multi-shop checkout.
- Supplier procurement and supplier marketplace.
- Full accounting/ERP.
- Advanced logistics fleet management.

# 26. Important Product Risks and Decisions to Validate

These points need further technical and business validation before implementation.

1. **Fully dynamic platform:** A no-code workflow and form builder is a major engineering feature. It should be implemented incrementally with safe, predefined action types and validation.
2. **Multiple industries and cities:** Launching three industries in multiple cities increases operational complexity. Shared functionality should be prioritized.
3. **Payments and settlements:** The chosen settlement model must be compatible with the payment gateway, merchant onboarding, refunds and applicable regulations.
4. **Refund permissions:** Business-controlled refunds must work within the platform's actual payment authorization model.
5. **Delivery-agent earnings:** Business-direct payment needs clear rules for platform agents working with multiple businesses.
6. **Live tracking:** Requires location permissions, background-location handling and battery-conscious updates.
7. **Privacy and legal compliance:** Customer consent, identity documents, location data, retention and deletion must be designed with applicable Indian privacy and payment requirements in mind.
8. **Business verification:** Define acceptable documents and review criteria for each business type.
9. **Customer complaints:** Business-only support is the selected model; platform-level intervention for serious fraud, safety or payment disputes still needs a policy decision.
10. **Subscription and commission:** Define how plans, commissions, taxes and payment settlements interact.

# 27. Recommended Next Development Stages

**Stage 1 – Product Definition**
- Review and approve this PRD.
- Confirm business rules.
- Identify MVP requirements.
- Finalize product name.

**Stage 2 – UI/UX Prototype**
- Customer mobile application.
- Business and operations mobile application.
- Super Admin web application.
- Design system.
- English and Tamil interface considerations.

**Stage 3 – Technical Planning**
- Architecture.
- Database design.
- API contracts.
- Authentication and permissions.
- Workflow configuration model.
- Payment and notification integrations.

**Stage 4 – Development**
- Build reusable platform foundation.
- Develop core customer and business modules.
- Implement initial industries.
- Build Super Admin configuration.
- Integrate payments and notifications.

**Stage 5 – Testing and Launch**
- Functional testing.
- Security testing.
- Business onboarding tests.
- Payment/refund tests.
- Location and delivery tests.
- Pilot launch.
- Production release.

---

**Document status:** Product discovery decisions consolidated. Technical design and implementation decisions are intentionally pending approval.