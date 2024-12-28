# APIOps Cycles Method - Prompts Guide

## Introduction

This guide provides prompts for each phase of the APIOps Cycles method. Each section includes clear objectives, detailed steps, practical examples, and measurable success criteria. The prompts are designed to guide API Product Managers through the entire APIOPs lifecycle while incorporating industry best practices and common scenarios.

## Phase 1: API Product Strategy

### 1.1 Customer Journey Mapping

**Objective:** Create a comprehensive map of the end-user's experience to identify strategic opportunities for API integration.

#### Steps

1. **Identify Key Touchpoints**
   - List all points where customers interact with your system/service
   - Include both digital and non-digital interactions
   - Document the sequence and relationships between touchpoints

   Example:
   ```
   E-commerce Journey:
   1. Product Search
   2. Product Details View
   3. Add to Cart
   4. Checkout Process
   5. Payment
   6. Order Confirmation
   7. Shipping Updates
   8. Delivery
   9. Returns/Support
   ```

2. **Document Gains and Pains**
   For each touchpoint, document:

   Gains Example (Product Search):
   - Quick access to relevant products
   - Accurate search results
   - Helpful filtering options
   - Real-time stock information

   Pains Example (Product Search):
   - Irrelevant search results
   - Slow search response
   - Missing product information
   - Outdated stock information

3. **Select Priority Journey**
   Choose one customer journey based on:
   - Business impact (revenue, cost savings)
   - Customer satisfaction impact
   - Technical feasibility
   - Strategic alignment

   Document your selection rationale:
   ```
   Selected Journey: Product Search to Purchase
   Rationale:
   - Highest impact on conversion rates
   - Clear technical opportunities for API integration
   - Significant pain points that can be addressed
   - Aligns with digital transformation goals
   ```

#### Success Criteria
- [ ] Complete journey map with all touchpoints identified
- [ ] Detailed gains and pains for each touchpoint
- [ ] Clear rationale for selected journey
- [ ] Validation from key stakeholders
- [ ] Identified API opportunities within the journey

### 1.2 API Value Proposition Canvas

**Objective:** Define clear value propositions for API consumers by mapping their needs to specific API features.

#### Steps

1. **Map API Consumer Tasks**
   
   Document primary tasks using this format:
   ```
   Task: [Task Name]
   Description: [Detailed description]
   Current Solution: [How it's done now]
   Frequency: [How often performed]
   Impact: [Business/Technical impact]
   ```

   Example:
   ```
   Task: Real-time Inventory Sync
   Description: Maintain accurate inventory levels across multiple sales channels
   Current Solution: Manual batch updates every 6 hours
   Frequency: Continuous
   Impact: Critical - affects order fulfillment and customer satisfaction
   ```

2. **Define Gain-Enabling Features**

   For each feature, document:
   ```
   Feature: [Feature Name]
   Type: [Functional/Non-functional]
   Gains Enabled:
   - [Specific gain 1]
   - [Specific gain 2]
   Metrics:
   - [How to measure success]
   ```

   Example:
   ```
   Feature: Real-time Stock Updates
   Type: Functional
   Gains Enabled:
   - Immediate inventory accuracy
   - Reduced overselling
   - Improved customer confidence
   Metrics:
   - Inventory accuracy rate
   - Number of failed orders due to stock issues
   - API response time
   ```

3. **Identify Pain-Relieving Features**

   Document pain points and solutions:
   ```
   Pain Point: [Description]
   Impact Level: [High/Medium/Low]
   Current Workarounds: [If any]
   Proposed Solution: [Feature description]
   ```

   Example:
   ```
   Pain Point: Inconsistent data formats across systems
   Impact Level: High
   Current Workarounds: Manual data transformation
   Proposed Solution: Standardized data transformation API endpoint
   ```

4. **Map Features to API Products**

   Create a feature mapping table:
   | Feature | Type | Implementation | Priority | Dependencies |
   |---------|------|----------------|-----------|--------------|
   | [Feature Name] | Buy/Build/Borrow | [Details] | [H/M/L] | [List] |

   Example:
   | Feature | Type | Implementation | Priority | Dependencies |
   |---------|------|----------------|-----------|--------------|
   | Stock Updates | Build | Real-time inventory API | High | Inventory System |
   | Payment Processing | Buy | Stripe API | High | Payment Gateway |
   | Analytics | Borrow | Existing Internal API | Medium | Analytics Platform |

#### Success Criteria
- [ ] Comprehensive task analysis for API consumers
- [ ] Clear mapping of features to gains and pains
- [ ] Prioritized feature list with implementation approach
- [ ] Validated assumptions with potential API consumers
- [ ] Measurable success metrics for each feature

### 1.3 API Business Model Canvas

**Objective:** Create a comprehensive business model for your API that ensures sustainable value delivery.

#### Steps

1. **API Value Proposition**
   
   Document your value proposition using this framework:
   ```
   Core Value: [Primary benefit]
   Target Consumer: [Specific API consumer segment]
   Key Differentiators:
   - [Differentiator 1]
   - [Differentiator 2]
   Value Metrics:
   - [Metric 1]
   - [Metric 2]
   ```

   Example:
   ```
   Core Value: Real-time inventory synchronization
   Target Consumer: E-commerce platforms and marketplaces
   Key Differentiators:
   - Sub-second response time
   - 99.99% accuracy guarantee
   - Built-in conflict resolution
   Value Metrics:
   - Reduction in overselling incidents
   - Improvement in order fulfillment rate
   ```

2. **API Consumer Segments**

   For each segment, document:
   ```
   Segment: [Name]
   Description: [Details]
   Key Needs:
   - [Need 1]
   - [Need 2]
   Usage Patterns:
   - [Pattern 1]
   - [Pattern 2]
   Growth Potential: [Analysis]
   ```

   Example:
   ```
   Segment: Enterprise E-commerce Platforms
   Description: Large-scale online retailers with multiple channels
   Key Needs:
   - High availability
   - Enterprise SLAs
   - Custom integration support
   Usage Patterns:
   - 24/7 operation
   - High volume (>1M calls/day)
   - Peak season scaling
   Growth Potential: High - expanding market with increasing API adoption
   ```

3. **Developer Relations**

   Create a comprehensive developer support plan:
   ```
   Documentation:
   - API reference
   - Integration guides
   - Code samples
   - Troubleshooting guides
   
   Support Channels:
   - Developer portal
   - Community forum
   - Direct support
   - Office hours
   
   Resources:
   - SDKs
   - Testing tools
   - Sandbox environment
   ```

4. **Channels**

   Document distribution strategy:
   ```
   Channel: [Name]
   Purpose: [Primary use]
   Target Segment: [Consumer segment]
   Features:
   - [Feature 1]
   - [Feature 2]
   Success Metrics:
   - [Metric 1]
   - [Metric 2]
   ```

5. **Benefits**

   Quantify benefits in these categories:
   ```
   Revenue Benefits:
   - Direct revenue: [Projections]
   - Indirect revenue: [Projections]
   
   Cost Savings:
   - Operational: [Estimates]
   - Integration: [Estimates]
   
   Strategic Benefits:
   - Market position
   - Innovation enablement
   - Partner ecosystem
   ```

6. **Key Activities**

   Create an activity matrix:
   | Activity | Frequency | Owner | Resources | Dependencies |
   |----------|-----------|-------|-----------|--------------|
   | [Activity] | [Frequency] | [Team] | [Resources] | [Dependencies] |

7. **Key Resources**

   Document required resources:
   ```
   Technical Resources:
   - Infrastructure
   - Development tools
   - Monitoring systems
   
   Human Resources:
   - Development team
   - Support team
   - Developer advocates
   
   Knowledge Resources:
   - Documentation
   - Training materials
   - Best practices
   ```

8. **Key Partners**

   Create a partner matrix:
   | Partner Type | Role | Value Exchange | Dependencies |
   |--------------|------|----------------|--------------|
   | [Type] | [Role] | [Value] | [Dependencies] |

9. **Costs**

   Document cost structure:
   ```
   Development Costs:
   - Initial development
   - Ongoing maintenance
   - Feature development
   
   Operational Costs:
   - Infrastructure
   - Support
   - Marketing
   
   Partner Costs:
   - Third-party services
   - Integration costs
   ```

#### Success Criteria
- [ ] Complete business model canvas with all components
- [ ] Clear value propositions for each consumer segment
- [ ] Detailed revenue and cost projections
- [ ] Identified key partnerships and resources
- [ ] Validated business model with stakeholders

## Phase 2: API Consumer Experience

### 2.1 Consumer Needs Validation

**Objective:** Validate and refine API consumer needs through direct engagement and feedback.

#### Steps

1. **Validate Value Proposition**
   
   Create validation interviews using this template:
   ```
   Interview Guide:
   
   Background:
   - Role/Company type
   - Current API usage
   - Integration experience
   
   Pain Points:
   - Current challenges
   - Workarounds
   - Impact of issues
   
   Feature Validation:
   - Proposed features review
   - Priority assessment
   - Missing capabilities
   
   Technical Requirements:
   - Preferred formats
   - Performance needs
   - Integration constraints
   ```

2. **Technical Requirements Gathering**

   Document technical requirements:
   ```
   Data Requirements:
   - Formats: [Preferred formats]
   - Volume: [Expected data volume]
   - Frequency: [Update frequency]
   
   Performance Requirements:
   - Latency: [Maximum acceptable]
   - Availability: [Required uptime]
   - Throughput: [Calls per second]
   
   Security Requirements:
   - Authentication: [Methods]
   - Authorization: [Levels]
   - Data protection: [Standards]
   ```

3. **Usability Features**

   Define developer experience requirements:
   ```
   Documentation:
   - API reference format
   - Code examples needed
   - Use case coverage
   
   Testing:
   - Sandbox requirements
   - Test data needs
   - Validation tools
   
   Support:
   - Response time needs
   - Support channels
   - Self-service tools
   ```

4. **Feature Prioritization Matrix**

   Create a prioritization framework:
   | Feature | Impact | Effort | Risk | Priority Score |
   |---------|---------|--------|------|----------------|
   | [Feature] | [H/M/L] | [H/M/L] | [H/M/L] | [Score] |

#### Success Criteria
- [ ] Completed validation interviews with target consumers
- [ ] Documented technical requirements with specific metrics
- [ ] Prioritized feature list based on consumer feedback
- [ ] Clear understanding of developer experience needs
- [ ] Validation of business model assumptions

## Phase 3: API Platform Architecture

### 3.1 Platform Evaluation

**Objective:** Assess platform capabilities and identify architectural requirements for successful API deployment.

#### Steps

1. **Data Location Mapping**

   Use this template for each data type:
   ```
   Data Type: [Name]
   Classification: [Security level]
   Current Location:
   - Primary: [Location]
   - Replicas: [Locations]
   
   Access Patterns:
   - Read frequency
   - Write frequency
   - Peak usage times
   
   Compliance Requirements:
   - Data residency
   - Retention rules
   - Privacy regulations
   ```

2. **API Producer/Consumer Mapping**

   Document each interaction:
   ```
   Producer System:
   - Name: [System name]
   - Type: [Internal/External]
   - Location: [Network location]
   - Capabilities: [List]
   
   Consumer System:
   - Name: [System name]
   - Type: [Internal/External]
   - Location: [Network location]
   - Requirements: [List]
   
   Interaction Patterns:
   - Protocol: [HTTP/Message Queue/etc.]
   - Frequency: [Rate]
   - Data volume: [Size]
   ```

3. **Regulatory Analysis**

   Create compliance matrix:
   | Requirement | Source | Impact | Implementation | Status |
   |------------|--------|---------|----------------|--------|
   | [Requirement] | [Regulation] | [Impact] | [Method] | [Status] |

#### Success Criteria
- [ ] Complete data location map with compliance requirements
- [ ] Documented producer/consumer interactions
- [ ] Identified regulatory requirements and solutions
- [ ] Assessment of current platform capabilities
- [ ] Gap analysis for required capabilities

### 3.2 Capacity Planning

**Objective:** Define and plan for the API's capacity requirements to ensure reliable performance.

#### Steps

1. **Business Transaction Analysis**

   Document each transaction type:
   ```
   Transaction: [Name]
   Description: [Details]
   
   Volume Metrics:
   - Average daily volume
   - Peak volume
   - Growth rate
   
   Resource Requirements:
   - CPU usage
   - Memory usage
   - Storage needs
   - Network bandwidth
   
   Dependencies:
   - Systems involved
   - External services
   - Database access
   ```

2. **Traffic Pattern Analysis**

   Create traffic models:
   ```
   Pattern Type: [Daily/Weekly/Seasonal]
   
   Baseline Traffic:
   - Average rate: [Calls/second]
   - Peak rate: [Calls/second]
   - Quiet period rate: [Calls/second]
   
   Growth Projections:
   - 3 month: [Rate]
   - 6 month: [Rate]
   - 12 month: [Rate]
   
   Special Events:
   - Type: [Event]
   - Expected impact: [Multiple of baseline]
   - Duration: [Time period]
   ```

3. **Scalability Planning**

   Document scaling strategy:
   ```
   Scaling Triggers:
   - CPU threshold: [%]
   - Memory threshold: [%]
   - Request queue length: [Number]
   - Response time: [ms]
   
   Scaling Rules:
   - Minimum instances: [Number]
   - Maximum instances: [Number]
   - Scale-out increment: [Number]
   - Cool-down period: [Time]
   
   Cost Implications:
   - Base cost: [Amount]
   - Scale unit cost: [Amount]
   - Peak cost: [Amount]
   ```

#### Success Criteria
- [ ] Documented transaction patterns and volumes
- [ ] Clear scaling thresholds and rules
- [ ] Resource requirements mapped to business needs
- [ ] Cost projections for different scaling scenarios
- [ ] Validation of capacity plan with stakeholders

### 3.3 Risk Assessment

**Objective:** Identify and plan mitigation strategies for potential risks to API operations.

#### Steps

1. **Availability Risk Analysis**

   Document availability scenarios:
   ```
   Scenario: [Description]
   Duration: [Time period]
   
   Impact Assessment:
   - Business impact: [Description]
   - Customer impact: [Description]
   - Financial impact: [Amount]
   
   Current Controls:
   - [Control 1]
   - [Control 2]
   
   Mitigation Strategy:
   - Primary: [Strategy]
   - Backup: [Strategy]
   - Recovery time objective: [Time]
   ```

   Example:
   ```
   Scenario: Complete API outage
   Duration: 1 hour
   
   Impact Assessment:
   - Business impact: Unable to process orders
   - Customer impact: Failed transactions
   - Financial impact: $10,000/hour
   
   Current Controls:
   - Load balancing
   - Health monitoring
   
   Mitigation Strategy:
   - Primary: Multi-region deployment
   - Backup: Cache critical data
   - Recovery time objective: 5 minutes
   ```

2. **Security Risk Analysis**

   Create security risk matrix:
   | Risk | Likelihood | Impact | Controls | Residual Risk |
   |------|------------|---------|-----------|---------------|
   | [Risk] | [H/M/L] | [H/M/L] | [Controls] | [H/M/L] |

   Example:
   | Risk | Likelihood | Impact | Controls | Residual Risk |
   |------|------------|---------|-----------|---------------|
   | SQL Injection | Medium | High | Input validation, Prepared statements | Low |
   | DDoS Attack | High | High | Rate limiting, WAF | Medium |

3. **Functionality Risk Analysis**

   Document functional risks:
   ```
   Risk Area: [Function]
   Potential Issues:
   - [Issue 1]
   - [Issue 2]
   
   Detection Methods:
   - [Method 1]
   - [Method 2]
   
   Recovery Procedures:
   - [Step 1]
   - [Step 2]
   
   Prevention Strategy:
   - [Strategy 1]
   - [Strategy 2]
   ```

#### Success Criteria
- [ ] Comprehensive risk register with impact assessment
- [ ] Documented mitigation strategies for each risk
- [ ] Clear recovery procedures for each scenario
- [ ] Cost-benefit analysis of mitigation strategies
- [ ] Stakeholder approval of risk management approach

## Phase 4: API Design

### 4.1 Data Requirements

**Objective:** Define comprehensive data requirements that meet both technical and business needs. Make sure to meet all success criteria.

#### Steps

1. **Core Concepts Definition**

   For each core concept:
   ```
   Concept: [Name]
   Description: [Details]
   
   Key Attributes:
   - Name: [Attribute]
     Type: [Data type]
     Required: [Yes/No]
     Validation: [Rules]
   
   Relationships:
   - [Related concept]
     Type: [One-to-one/Many-to-many/etc.]
     Description: [Details]
   
   Business Rules:
   - [Rule 1]
   - [Rule 2]
   ```

2. **Data Standards Mapping**

   Document applicable standards:
   ```
   Standard: [Name]
   Scope: [Industry/National/etc.]
   
   Required Fields:
   - [Field 1]
   - [Field 2]
   
   Format Requirements:
   - [Requirement 1]
   - [Requirement 2]
   
   Validation Rules:
   - [Rule 1]
   - [Rule 2]
   ```

3. **Data Freshness Requirements**

   Define freshness needs:
   ```
   Data Type: [Name]
   Update Frequency: [Time]
   
   Staleness Impact:
   - Business: [Impact]
   - Technical: [Impact]
   
   Refresh Strategy:
   - Method: [Strategy]
   - Trigger: [Event/Time]
   - Validation: [Process]
   ```

#### Success Criteria
- [ ] Documented core concepts with attributes
- [ ] Mapped applicable data standards
- [ ] Defined data freshness requirements
- [ ] Validated requirements with stakeholders
- [ ] Clear documentation of business rules
- [ ] Defined JSON Schema specification
- [ ] Defined JSON data examples, that match JSON Schema specification

### 4.2 Request/Response Design

**Objective:** Design clear, consistent, and efficient API interactions. Make sure to meet all success criteria.

#### Steps

1. **Request Design**

   For each endpoint:
   ```
   Endpoint: [Path]
   Method: [HTTP Method]
   
   Request Parameters:
   - Name: [Parameter]
     Location: [Path/Query/Header/Body]
     Type: [Data type]
     Required: [Yes/No]
     Description: [Details]
     Example: [Value]
   
   Validation Rules:
   - [Rule 1]
   - [Rule 2]
   
   Rate Limiting:
   - Default: [Rate]
   - Burst: [Rate]
   ```

2. **Response Design**

   For each response:
   ```
   Status Code: [Code]
   Description: [Details]
   
   Response Body:
   - Field: [Name]
     Type: [Data type]
     Description: [Details]
     Example: [Value]
   
   Headers:
   - Name: [Header]
     Description: [Details]
     Required: [Yes/No]
   
   Caching:
   - Strategy: [Method]
   - Duration: [Time]
   ```

3. **Error Handling**

   Document error responses:
   ```
   Error Category: [Type]
   Status Code: [Code]
   
   Response Format:
   {
     "code": "string",
     "message": "string",
     "details": [
       {
         "field": "string",
         "issue": "string"
       }
     ]
   }
   
   Error Scenarios:
   - Scenario: [Description]
     Response: [Example]
   ```

#### Success Criteria
- [ ] API contract is based on 4.1 Data Requirements
- [ ] Complete API contract in OpenAPI format
- [ ] Consistent error handling across endpoints
- [ ] Clear validation rules and examples
- [ ] Documented rate limiting and caching
- [ ] Peer review of API design

### 4.3 Asynchronous API Design

**Objective:** Design effective event-driven API interactions for real-time data and long-running processes. Make sure to meet all success criteria.

#### Steps

1. **Event Definition**

   For each event:
   ```
   Event: [Name]
   Description: [Details]
   
   Payload:
   - Field: [Name]
     Type: [Data type]
     Required: [Yes/No]
     Description: [Details]
   
   Triggering Conditions:
   - [Condition 1]
   - [Condition 2]
   
   Delivery Requirements:
   - Ordering: [Required/Not required]
   - Persistence: [Duration]
   - Retry policy: [Strategy]
   ```

2. **Subscription Management**

   Document subscription handling:
   ```
   Subscription Process:
   - Authentication: [Method]
   - Authorization: [Rules]
   - Rate limiting: [Limits]
   
   Configuration Options:
   - Filters: [Available filters]
   - Delivery method: [Methods]
   - Format options: [Formats]
   
   Management APIs:
   - Create subscription
   - Update subscription
   - Delete subscription
   - List subscriptions
   ```

3. **Event Processing Rules**

   Define processing requirements:
   ```
   Processing Stage: [Name]
   
   Input Validation:
   - [Rule 1]
   - [Rule 2]
   
   Transformation Rules:
   - [Rule 1]
   - [Rule 2]
   
   Error Handling:
   - Scenario: [Description]
   - Action: [Response]
   ```

#### Success Criteria
- [ ] API contract is based on 4.1 Data Requirements
- [ ] Complete AsyncAPI specification
- [ ] Defined event schemas and examples
- [ ] Clear subscription management process
- [ ] Documented error handling scenarios
- [ ] Validated event processing rules

### 4.4 MVP Prioritization

**Objective:** Prioritize API features for initial release while ensuring extensibility for future growth.

#### Steps

1. **Feature Analysis**

   Create feature evaluation matrix:
   | Feature | Business Value | Technical Complexity | Dependencies | MVP Status |
   |---------|---------------|---------------------|--------------|------------|
   | [Feature] | [H/M/L] | [H/M/L] | [List] | [Yes/No] |

2. **MVP Scope Definition**

   Document MVP requirements:
   ```
   Core Capabilities:
   - [Capability 1]
   - [Capability 2]
   
   Success Metrics:
   - [Metric 1]: [Target]
   - [Metric 2]: [Target]
   
   Limitations/Constraints:
   - [Limitation 1]
   - [Limitation 2]
   
   Future Considerations:
   - [Enhancement 1]
   - [Enhancement 2]
   ```

3. **Technical Debt Assessment**

   Document technical decisions:
   ```
   Decision: [Description]
   
   Rationale:
   - [Reason 1]
   - [Reason 2]
   
   Impact:
   - Short term: [Impact]
   - Long term: [Impact]
   
   Mitigation Plan:
   - [Strategy 1]
   - [Strategy 2]
   ```

#### Success Criteria
- [ ] Clear MVP feature set defined
- [ ] Documented decision rationale
- [ ] Identified future enhancements
- [ ] Stakeholder agreement on scope
- [ ] Technical debt management plan

## Phase 5: API Audit

Use the prompt from the [api-audit-execution-claude-standalone.md](./api-audit-execution-claude-standalone.md) file.

## Phase 6: API Publishing

### 6.1 Publication Preparation

**Objective:** Ensure successful API deployment and adoption through comprehensive documentation and support.

#### Steps

1. **Documentation Package**

   Create documentation set:
   ```
   Technical Documentation:
   - API reference
   - Authentication guide
   - Error handling guide
   - Rate limiting details
   
   Integration Guides:
   - Getting started
   - Best practices
   - Sample code
   - Use cases
   
   Support Materials:
   - FAQ
   - Troubleshooting guide
   - Change log
   - Support contact info
   ```

2. **Developer Portal Setup**

   Configure portal features:
   ```
   Portal Components:
   - API documentation
   - Interactive console
   - Authentication management
   - Usage analytics
   
   Self-Service Features:
   - API key generation
   - Subscription management
   - Usage monitoring
   - Support tickets
   ```

#### Success Criteria
- [ ] Complete documentation package
- [ ] Functional developer portal
- [ ] Testing environment ready
- [ ] Support processes defined
- [ ] Monitoring tools configured

## Phase 7: API Adoption

### 7.1 Adoption Strategy

**Objective:** Drive successful API adoption through effective onboarding and support.

#### Steps

1. **Onboarding Process**

   Define onboarding journey:
   ```
   Stage 1: Initial Access
   - Account creation
   - API key generation
   - Documentation access
   
   Stage 2: First Integration
   - Sample code review
   - Test environment setup
   - Initial API calls
   
   Stage 3: Production Launch
   - Production credentials
   - Going live checklist
   - Support handoff
   ```

2. **Success Metrics**

   Define KPIs:
   ```
   Adoption Metrics:
   - New integrations per month
   - Active consumers
   - API call volume
   
   Quality Metrics:
   - Error rates
   - Response times
   - Availability
   
   Support Metrics:
   - Time to first successful call
   - Support ticket volume
   - Resolution time
   ```

3. **Feedback Loop**

   Establish feedback process:
   ```
   Feedback Channels:
   - Developer surveys
   - Usage analytics
   - Support tickets
   - Community forum
   
   Analysis Process:
   - Data collection
   - Pattern identification
   - Priority assessment
   
   Action Items:
   - Feature requests
   - Documentation updates
   - Process improvements
   ```

#### Success Criteria
- [ ] Defined onboarding process
- [ ] Established success metrics
- [ ] Active feedback channels
- [ ] Regular adoption reviews
- [ ] Continuous improvement plan
```
