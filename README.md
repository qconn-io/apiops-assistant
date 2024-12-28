# APIOps Assistant

This project is an AI-powered assistant designed to guide API Product Managers through the APIOps Cycles method. It utilizes various tools and checklists to ensure efficient, customer-centric, and business-objective-aligned API development and management.

## Project Structure

The project is organized into directories, each serving a specific purpose in the APIOps process. It includes specification documents, guidelines, instructions, and prompts for successful API development.

**Directories:**

* **context**: Foundational files
    * **api_design_skeletons**: Template files for API specifications (OpenAPI (REST) and AsyncAPI)
    * **api_standards**: Guidelines and checklists for API development
    * **instructions**: System instructions for the AI assistant
* **prompts**: Specific prompts for different APIOps lifecycle tasks
* **storyline**: Example use cases and scenarios for APIs

## Key Components

### API Design Skeletons

- `api_design_skeletons`: Directory containing templates for defining APIs
  - `AsyncSkeleton.yaml`: Template for defining asynchronous APIs (AsyncAPI) with sections for:
    - Metadata (title, version, description)
    - Server configurations
    - Channels and messages
    - Security schemes
  - `RestSkeleton.yaml`: Template for defining RESTful APIs (OpenAPI) with sections for:
    - Metadata (title, description, contact)
    - Server URLs and security
    - Paths and endpoints (CRUD)
    - Parameters, request bodies, and responses
    - Schemas, error objects, and examples
    - Security schemes

### API Standards

- `api_standards`: Guidelines, documentation, and best practices for API development:
  - `rest_guidelines.md`: Outlines guidelines for designing REST APIs, including:
    - Naming conventions
    - Localization and internationalization
    - Security best practices
    - Versioning strategies
    - Error handling and response codes
    - Filtering, paging, and hypermedia links
    - Time selection and sorting
  - `apiops-method-full.md`: Comprehensive document detailing the APIOps Cycles method, providing guidance for each phase, from strategy to adoption
  - `apiops-method-summary.md`: Summarized view of the APIOps Cycles method, highlighting core principles, key concepts, and API lifecycle stages.

### Instructions

- `instructions.txt`: Specific instructions and role description for the AI assistant, defining its expertise and behavior.

### Prompts

- `prompts`: Directory containing prompts to guide the AI assistant:
  - `api-audit-execution-claude-standalone.md`: Detailed guide for planning and executing an API audit, referencing checklists from the APIOps method.
  - `apiops-method-prompts-claude-verified.md`: Detailed prompts for each APIOps Cycles method phase, including objectives, steps, examples, and success criteria.

### Storyline

- `discounts-api-storyline.md`: Narrative-style storyline and requirements for a Discounts API, including personas and key requirements for marketing flexibility, checkout performance, compliance, technical architecture, and future expansion.

## APIOps Cycles Method

The APIOps Cycles method, described in `apiops-method-full.md` and `apiops-method-summary.md`, consists of the following core stations:

1. **API Product Strategy**: Aligns APIs with business goals and customer needs.
2. **API Consumer Experience**: Prioritizes usability and adoption based on user and developer needs.
3. **API Platform Architecture**: Ensures a secure and scalable API infrastructure.
4. **API Design**: Creates well-documented and user-friendly APIs.
5. **API Audit**: Validates API quality and compliance.
6. **API Publishing**: Makes APIs discoverable and accessible.
7. **API Adoption**: Drives usage and ensures APIs meet business goals.

## Usage

This AI Assistant project assists API Product Managers in various ways:

- **API Design**: Generate API specifications using the provided templates.
- **API Audit**: Conduct thorough API audits using the guidelines and checklists.
- **APIOps Guidance**: Follow the APIOps Cycles method with prompts and instructions.
- **Story-Driven Development**: Understand and address stakeholder needs through example scenarios.

This project is a comprehensive resource for API development and management, promoting best practices and ensuring APIs deliver value.