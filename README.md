# Reducing-Payment-Drop-Offs-in-Online-Flight-Booking
Case Study | Business Analysis · Product Analytics · UX Optimization
Live Dashboard:https://public.tableau.com/views/projectflightbookingfunnel/Home?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
Project Overview

AeroEase is an imaginary online flight booking platform facing a critical business challenge:
high user drop-offs at the payment stage, resulting in significant revenue loss despite strong performance in earlier funnel stages.

This project analyzes payment-stage friction using dashboards and proposes data-backed UX and system improvements, supported by a Business Requirements Document (BRD), AS-IS & TO-BE process flows, and a Functional Requirements Document (FRD).

🎯 Problem Statement

A significant proportion of users who reach the payment stage abandon their booking due to:

Payment friction

Technical failures

Poor error handling

UX gaps

This leads to high revenue loss, even though users show strong intent by completing search and selection steps.

📊 Evidence from Dashboard Analysis

Key insights derived from the analytical dashboard:

🔴 Highest drop-off occurs at the Payment stage

✅ UPI performs best with ~69% success rate

⚠️ Wallet & Net Banking experience ~50% drop-off

📱 Mobile page load time is significantly higher than desktop

🇮🇳 India contributes the highest absolute drop-offs

🌐 Browser errors are concentrated on Chrome & Firefox

These insights confirmed that payment experience, not demand, is the core issue.

🧠 Business Objective

Reduce payment page drop-off rate from 63% to 45%

Achieve an 18 percentage point reduction within 3 months

Improve overall booking conversion and revenue realization

🧩 Solution Strategy (High Level)

The solution focuses on reducing friction and failure recovery effort at the payment stage through:

Smart retry logic

Payment method prioritization

UX improvements

Contextual error handling

Performance optimization

📄 Business Requirements Document (BRD)

The BRD defines what needs to be achieved from a business perspective.

Key BRD Sections:

Executive Summary

Background & Problem Analysis

Project Scope (In-Scope / Out-of-Scope)

Stakeholder Analysis

High-Level Functional Requirements

High-Level Non-Functional Requirements

Assumptions & Constraints

Success Criteria & KPIs

In-Scope Highlights:

Payment page UX redesign

Smart payment retry mechanism

Payment method recommendation

Contextual & actionable error messaging

Out-of-Scope:

Pricing or fare calculation changes

Airline inventory integration

Loyalty programs or discounts

🔁 Process Flow Documentation
1️⃣ AS-IS Flow (Current State)

The existing payment flow suffers from:

Manual re-entry after failures

Generic error messages

No retry or fallback guidance

High user effort during failures

📌 Purpose:
Used in the BRD to highlight current pain points and justify change.

2️⃣ TO-BE Flow (Future State)

The optimized flow introduces:

Context-aware payment method recommendation

Auto-retry for soft failures

One-click retry (no data re-entry)

Alternate payment suggestions for hard failures

Fare lock with countdown timer

Clear booking confirmation

📌 Purpose:
Detailed in the FRD to guide system implementation.

Flow diagrams are created using Lucidchart and referenced in documentation.

⚙️ Functional Requirements Document (FRD)

The FRD defines how the system will be built.

Key Features Covered:

Payment detail preservation

Failure type classification (Soft vs Hard)

Auto-retry logic

Alternate payment prioritization

Contextual error messages

Performance and security requirements

Non-Functional Highlights:

Payment page load time < 2.5 seconds (mobile)

Payment API success rate > 99.5%

PCI-DSS compliance

High availability & fault tolerance

📉 Justification for 18% Drop-Off Reduction

The projected improvement is derived by mapping solutions to known failure causes:

Improvement Area	Expected Impact
Auto-retry (Soft failures)	~5%
One-click retry	~4%
Payment method prioritization	~4%
Contextual error handling	~3%
Fare lock & trust signals	~2%
Total Estimated Reduction	~18%

Benchmarks are aligned with industry practices from platforms like MakeMyTrip, Ixigo, and Google Pay.

📈 Success Metrics

Payment drop-off rate

Payment success rate

Retry success rate

Overall booking conversion

Revenue leakage reduction

Mobile payment error rate

🛠 Tools & Skills Used

Power BI – Funnel & payment analysis dashboard

SQL – Funnel metrics & failure analysis

Lucidchart – AS-IS & TO-BE process flows

Business Analysis – BRD & FRD documentation

UX Benchmarking – Competitor gap analysis
