# The APIOps Cycles Method

## API Product Strategy
*For Architects, API Product Managers, Business Leaders*

The API Product Strategy phase is the initial step in the core API lifecycle of the APIOps Cycles method, focusing on aligning your API initiatives with business objectives and customer needs. This phase utilizes tools like the Customer Journey Map, API Value Proposition Canvas, and API Business Model Canvas to ensure your APIs deliver tangible value.

### Customer Journey Map
Understanding the customer's experience is crucial. A Customer Journey Map visualizes the steps a customer takes when interacting with your business, highlighting key touchpoints and potential areas for API integration.

### API Value Proposition Canvas
This tool helps identify which API features will provide value to consumers by mapping customer activities to their journeys. It ensures your API offerings align with user expectations and business goals.

By mapping tasks, gains, and pains, it ensures your API delivers value that resonates with its users, whether they are developers, partners, or internal teams.

#### Tips for Effective Use
* Collaborate with stakeholders: Use this canvas in workshops to align API providers and consumers
* Focus on API consumers: Think of your API's value proposition from the perspective of those who will use it
* Iterate: Update the canvas regularly to reflect evolving requirements and priorities

#### Step-by-Step Instructions

1. **Map Consumer Tasks (Start Here)**
   * Identify the key tasks or touchpoints in your consumers' journey where your API will play a role
   * Example: "Book a ticket," "Fetch customer details," or "Integrate payment processing"

2. **Define Gain-Enabling Features**
   * List the features that help API consumers achieve their goals or improve their experience
   * Focus on both functional (e.g., faster data access) and non-functional (e.g., reliable availability) gains
   * Example: "Real-time data updates," "Seamless integration," or "Improved response times"

3. **Identify Pain-Relieving Features**
   * Note down features that address your consumers' frustrations, risks, or challenges
   * Think of obstacles your API can solve, such as system errors, security concerns, or performance bottlenecks
   * Example: "Automatic error correction," "Enhanced security layers," or "Transparent rate limits"

4. **Connect API Products to Features**
   * Map the identified features to API products (or services) you'll deliver. Indicate whether these are:
     * Buy: Third-party APIs or services you will integrate
     * Build: Custom APIs or components you'll develop in-house
     * Borrow: Existing APIs you'll repurpose or extend
   * Example: "Authentication service," "Flight search API," or "Notification system"

#### What's Next?
Once you've completed the API Value Proposition Canvas:
* Move to the next station: Use the API Business Model Canvas to refine the API's value, target audience, and revenue model
* Test your assumptions: Validate the listed tasks, gains, and pains with real API consumers to ensure accuracy

### API Business Model Canvas
The API Business Model Canvas allows you to explore API opportunities by summarizing your API strategy on a single page. It covers aspects like consumer segments, value propositions, channels, and revenue streams, providing a comprehensive overview of your API's business model.

Use the API business model canvas to explore one API opportunity. Pick the opportunity with the highest impact on the customer journey.

#### Tips for Effective Use
* Collaborate across teams: Involve stakeholders from business, technical, and operational teams to fill out this canvas
* Iterate frequently: Review and refine your API business model as consumer needs and organizational priorities evolve
* Connect with the big picture: Use this canvas alongside others, like the API Value Proposition Canvas, to ensure alignment

#### Step-by-Step Instructions

1. **API Value Proposition**
   * Start by summarizing the value proposition of one API, as defined in the API Value Proposition Canvas
   * Focus on what makes this API valuable to its consumers, such as key features or capabilities
   * Example: "Provide real-time flight availability data for seamless booking experiences"

2. **API Consumer Segments**
   * Define the key groups or personas who will consume your API
   * Consider developers, partner organizations, internal teams, or third-party applications
   * Example: Travel agencies, airline partners, and internal analytics teams

3. **Developer Relations**
   * Identify how you will build relationships with developers and other API consumers
   * Highlight support mechanisms such as onboarding, documentation, or community engagement
   * Example: A dedicated developer portal with tutorials, an FAQ, and API testing tools

4. **Channels**
   * Outline the distribution channels for your API. How will consumers discover, access, and use your API?
   * Channels could include API marketplaces, direct partnerships, or internal platforms
   * Example: Publishing the API on a travel industry marketplace and hosting it on your developer portal

5. **Benefits**
   * Quantify the benefits your API will deliver, both direct and indirect
   * These could include revenue generation, cost savings, or strategic advantages
   * Example: Increased bookings through seamless integrations or reduced support costs via self-service tools

6. **Key Activities**
   * List the core activities required to deliver and maintain the API
   * These might include development, testing, operations, and marketing efforts
   * Example: Continuous integration and deployment (CI/CD), monitoring, and API promotion

7. **Key Resources**
   * Identify the resources needed to provide and scale the API
   * These could include infrastructure, developer expertise, or documentation tools
   * Example: Cloud hosting, API management platforms, and skilled developers

8. **Key Partners**
   * Define the partners critical to delivering the API successfully
   * These could be technology providers, business partners, or regulatory bodies
   * Example: Cloud providers, integration partners, or compliance consultants

9. **Costs**
   * Analyze the costs associated with building, maintaining, and scaling the API
   * Consider infrastructure, staffing, and marketing expenses
   * Example: Hosting costs, API gateway fees, and salaries for the development team

## API Consumer Experience
*For API Product Managers*

Understand your audience. Design APIs that developers want to use and that deliver business value. The API Consumer Experience station builds directly on the work completed in the API Product Strategy station, where you identified the API's core value proposition, business goals, and consumer segments.

### Build on the API Business Model Canvas
By refining the insights from the API Business Model Canvas, this station helps you:
* Deeply understand the consumer segments identified earlier
* Translate business-level insights into actionable technical and usability requirements
* Prioritize features that enhance developer satisfaction and increase API adoption

### Understand API Consumer Needs
* Validate the API Value Proposition pains and gains with your actual or potential API consumers
* Ask detailed questions on preferrable data formats, performance requirements, etc.
* Identify the specific pain points, expectations, and goals of developers or systems using the API
* Gather and prioritize technical requirements, usability features, and documentation needs

### Next Steps
Proceed to the API Platform Architecture station to summarize the needs and design infrastructure that supports these consumer needs at the required scale. Ensure alignment between API consumer requirements and the platform's capabilities to provide seamless performance and reliability.

## API Platform Architecture
*For Architects, API Product Managers, Business Leaders*

The API Platform Architecture station focuses on ensuring that your API fits seamlessly into your existing platform architecture or establishes clear requirements to guide necessary architectural changes. It balances the core needs of API producers, API consumers, and broader organizational goals, providing a foundation for scalability, security, and performance.

### Evaluate the Existing Platform or Environment
Assess how well your current platform architecture supports the API's functional and non-functional requirements.

Key focus areas:
* Data and Systems: Are the necessary systems and data already integrated into the platform? If not, what gaps exist?
* Regulatory Compliance: Are there geographic or industry-specific rules (e.g., GDPR, HIPAA)?

#### Use the Locations of Data and Systems Canvas
How to Use:

1. **Map Data Locations:**
   * Identify where your data (both master and copies) resides within the following scopes:
     * Company Network: Internal systems and storage
     * Partner Network: Systems managed by third-party providers or collaborators
     * Country Network: Data localized for specific geographies
     * Global Network: Cloud or international data systems

2. **Map API Producers and Consumers:**
   * For each network scope, list the API producers and API consumers:
     * Producers: Teams or systems providing the API
     * Consumers: Teams, applications, or partners consuming the API

3. **Analyze Regulatory and Network Constraints:**
   * Assess compliance requirements, such as GDPR or country-specific data localization laws
   * Identify network limitations or inefficiencies that could affect API delivery

**Output:**
A comprehensive view of data and system locations, regulatory considerations, and consumer-producer interactions to guide platform architecture decisions.

### Define Capacity Requirements for the API
From the API Value Proposition and API Consumer Needs, use any existing traffic patterns and business knowledge of customer behavior trends to identify specific platform requirements, such as:
* Performance: Can the platform handle the expected load (including peak traffic)?
* Scalability: What peak loads or transaction rates should the platform support?
* Latency: What are the tolerable delays for API consumers?

#### Use the Capacity Canvas
How to Use:

1. **Identify Business Transactions Driving API Traffic:**
   * Document the core business processes that generate API requests (e.g., user logins, data synchronization, payment processing)
   * Estimate transaction frequency and expected growth rates

2. **Plot Traffic Patterns:**
   * Use the graph to map expected traffic over time:
     * X-Axis: Time intervals (e.g., 1 month, 6 months, 12 months)
     * Y-Axis: Business transaction volume or API calls
   * Include regular fluctuations (e.g., daily peaks) and anticipated surges (e.g., seasonal traffic or marketing campaigns)

3. **Plan for Scalability:**
   * Based on the traffic forecast, define infrastructure requirements:
     * Compute power (e.g., scaling servers)
     * Storage needs
     * Network capacity
   * Align your scaling strategy with the API's expected lifecycle

**Output:**
A data-driven plan for scaling the API platform, ensuring it meets performance requirements under varying traffic loads.

### Assess Risks and Mitigation
Prioritize potential risks based on business impact:
* Availability risks: What happens if the API goes down?
* Security risks: What are the consequences of unauthorized access or data breaches?
* Functionality risks: What if the API delivers incorrect or outdated data?

#### Use the Business Impact Canvas
How to Use:

1. **Define Potential Risks:**
   * Availability Risks: What happens if the API is unavailable for 1 minute, 1 hour, or 1 day?
   * Security Risks: What are the consequences of unauthorized access, data breaches, or inappropriate permissions?
   * Functionality Risks: What if the API delivers outdated, incorrect, or incomplete data?

2. **Assess Business Impacts:**
   * For each type of risk, evaluate the impact on your business
   * Examples:
     * Availability: Loss of customer transactions or operational delays
     * Security: Regulatory fines, brand reputation damage, or customer trust loss
     * Functionality: Failed integrations, incorrect reports, or poor user experiences

3. **Document Mitigation Strategies and Costs:**
   * Identify ways to reduce or eliminate each risk (e.g., backup systems, stricter security protocols)
   * Estimate the cost of implementing each mitigation strategy, and weigh it against the potential impact

**Output:**
A clear overview of key risks, their potential impacts, and mitigation strategies to inform architectural decisions.

## API Design
*For Architects, API Developers, API Product Managers*

The API Design station is where you refine your API concept into actionable, detailed design specifications. This phase builds upon the insights from API Product Strategy and API Consumer Experience stations, incorporating the foundational architecture and requirements.

### Refine Data Requirements
Use the Data Requirements Canvas to ensure that the API handles critical data efficiently:
* Identify the top 5 concepts your API needs to support
* Clarify any industry, national, or company-wide standards for data
* Define common identifiers or must-have attributes (e.g., customer IDs, timestamps)
* Specify how fresh the data must be, based on the consumer's expectations
* Answer key questions API consumers need addressed (e.g., reports, metrics, or responses)

#### Top 5 Concepts
Start with the top 5 concepts, then continue to validate them with the questions.

The top 5 concepts are logical concepts, usually nouns, that make up the core of the API under design. For example, products, customers, ingredients, and locations are core concepts for a food delivery API.

Sometimes you will notice at this stage, what you thought would be one API or one endpoint, is actually splitting into several.

After you have the initial core concepts, start working your way clockwise in the template.

##### What Questions the API Consumers Need Answers To?
Write down questions like "What products can be delivered to my location in under 30 minutes?". These will form the bases of your GET-requests, in this case for "products" -resource aka. endpoint. Your variables will be location (possible address or geolocation) and delivery time (in minutes). Your response will contain a list of products, that you have to identify somehow.

##### International, National, Industry Specific or Company Wide Data Standards?
You already identified products, location and time as concepts. What regulations or standards are related to these, for example ISO-standards or legal requirements? Good starting point are the schemata in schema.org where most concepts have been described as a ready made schema with examples and proper standards.

Products is a notoriously tricky concept for standards, because each industry has it's own set of standards for products, even though there are some globally standard identifiers.

##### Common Identifiers and Required Attributes?
* The products and locations need to be identified, for sure. But how? Location for example can be stored as co-ordinates or with address schema containing street address and ISO code for country.
* Which attributes do you have to really have to ask the question? Do you always have to give location? Probably. But what about the delivery time? Is some default time used, if it isn't given?
* What about the response? What is the minimum information needed about products in this case. Is it enough to return identifier, or should you also include product name in the response to make it easier to the client consuming the API. This is ok for GET requests, but do we also offer an API endpoint for creating products or orders? What are the minimum requirements then?

##### How Fresh the Data Needs to Be?
How fresh is fresh data is always a relative question. In this example case all we know is that the food delivered as a result of the API must be fresh. The list of products might be quite stable, but the availability and queue size of orders waiting to be delivered might vary. Is 5 minutes enough or should it be 30 seconds or 5 seconds? All of these options have different requirement on integrations, humans updating the information or processing the queue and the customer experience.

##### Considerations for Data Requirements
* Private APIs are used by one application, internal APIs by several internal applications. They contain attributes and data that are business-critical and confidential.
* Partner APIs are available for third-party organizations under partnership terms and conditions. Partner APIs may contain partner-specific or customer data which is not available in public. 
* Public APIs allowing self-registration can require authentication. Usually public APIs contain data that has access to the underlying technology or data can use to access their own or any available data. Some public APIs may offer data licensed as open data, but an open API does not always offer open data.

#### How to Use the Request & Response Template
Request & Response is the typical pattern for any APIs, including REST APIs. It may not always be the most efficient, though.

A lot of polling is needed to keep the data fresh, because the API consumer won't know if the data has changed in the API provider side.

Start from the left-top corner by designing the request and then design the right-bottom corner, the response.

What needs to be done in the middle to perform the request and clean the response, depends on the systems and data sources involved.

##### The Request
Use bullet points and example data to describe the attributes needed for the request. Dissect the questions from the Data requirements -template as requests (one question should be one request).

Also creating or updating data requires a request, but move to this after processing the questions (the GET -requests) first.

##### The Response
Use bullet points and example data to describe the attributes needed for the response. Describe what the response will contain. Remember the response is the "answer" to your "question" set in the request.

In case the request contains data to be created or sent for processing or updates, the response is possibly empty or contains only an identifier.

##### Perform Request
The systems, data sources and algorithms, possibly even other APIs that need to be used to handle the request.

Because we are still on the business language and logical level, write the processing rules in a human language sentence: "Check which cooks have an order queue that will empty in given amount of minutes (deadline) and what products (pizza, pasta, chinese) are they able to make?"

##### Response Values
This step is about cleaning the values and combining different data sources so that the performed results can be sent as response. This step can be optional, depending on need. Use it in situations where it's clear that some identifiers, categories or for example time stamps coming from the underlying systems or logic need some standardizing or cleaning up. Use this step also to describe filtering out data and operations due to access rights of the user.

#### How to Use the Events Template
The events (or push or hooks) template is used for a subscription based model where the API provider will inform the API consumer when some condition is met and data or state is changed.
* Request subscription (at the top) is done once, when the API consumer subscribes to hear about specific events.
* Process event layer (middle) is for describing triggers and processing rules for specific event, for example when product delivery is confirmed.
* Subscription removal (bottom) is used for describing how the subscription is removed when the API consumer no longer is interested in the events.

### Define Interaction Scenarios
Leverage tools like the API Design with Requests and Responses Canvas:
* Document realistic scenarios where your API will be used
* Define the consumer's requests, including:
    * Expected payloads, headers, and supported HTTP verbs
* Describe the API provider's responses, covering status codes, data payloads, and error handling
* Validate these scenarios with API consumers and identify any gaps

For asynchronous APIs, use the API Design with Events and Hooks Canvas:
* Specify event subscriptions (e.g., how consumers subscribe)
* Outline how events will flow, including:
    * Event triggers and message payloads
    * Feedback loops for event acknowledgment or error handling

### Prioritize for MVP API Contract
Map the API design to business goals, focusing on essential functionalities for the Minimum Viable Product (MVP) for your API contact i.e. the technical interface design using standards such as OpenAPI or AsyncAPI:
* Ensure the API aligns with previously defined consumer segments and use cases
* Integrate constraints from the API Platform Architecture station, such as:
    * Latency limits, data formats, or security protocols
* Use iterative feedback loops to refine and finalize designs
* Create the API contract using your organization's style guide, such as the OpenAPI standard

#### REST API Design Guide
How should endpoints i.e. the resources that our API allows the API consumers to use, be named? What features and thus endpoints should be included in the same API? To version or not and how?

There are no actual standards for how endpoints etc. should be named. There are some conventions and best practices that help the APIs to be RESTful. These conventions make the API easy to understand by humans as well as programming and integration tools. Design with the next phase, API Audit criteria in mind. When designing REST APIs, use the REST API style guide as your guideline.

At first, add only the endpoints and data attributes that you know are necessary. This reduces the need for versioning, support and maintenance. When an API is versioned the API consumers are at risk of having to make changes. There are many APIs that have succeeded in avoiding breaking changes.

##### Overview
Our goal is consistency, maintainability, and best practices across applications. APIOps aim to balance a truly RESTful API interface with a positive developer experience (DX).

In a nutshell:
* Keep APIs' functionalities as simple as possible. The endpoints do only one thing, but they do it well.
* Avoid overlapping functionalities between different APIs.
* In case of an error include the API response verbose description. Include also a description of the erroneous parameter value, if it is feasible.
* Implement in each API (or bundle of APIs) ability to generate its own machine-readable document about its functionality.
* API must have support for the OPTIONS endpoint, which is needed for example in a preflight request in SwaggerUI

##### Minimum Developer Experience
* Each API must have a descriptive title
* The description of API has to be sufficient
* Each API must have documentation, either an OpenAPI file or other standard specification that is supported by the API management solution used
* Each API should have a getting started section to provide a low learning curve and fast 1st positive experience for the consumer

##### The Format of API Specification
Use the most recent OpenAPI version supported by the API management platform to describe your API, unless you are developing your API using GraphQL, AsyncAPI, gRPC or some other standard. OpenAPI Specification (Wikipedia) originally known as the Swagger Specification, is a specification for machine-readable interface files for describing, producing, consuming, and visualizing RESTful Web services.

Information about supported versions:
* IBM API Connect
* Azure API management - see also restrictions and known issues
* AWS API Gateway

Use examples-attribute with JSON schemas (validated) to provide automatically generated documentation and smart mock data to help use the API.

##### Naming Standards
* All URI parts including resource names are written in small letters
* Use only camelCase in all attribute (field) names
* Do not use special characters in URI or in attribute names
* Use English only in OpenAPI specification
* Use common legally used or industry-specific (not company-specific) words about resources and attributes. Refer to ISO standards as a primary source, then use WTO, EU or other trade area-specific vocabularies, http://schema.org/ or industry-specific vocabularies for naming. As a last resort, refer to company-specific vocabularies before inventing your own
* Avoid using generic names like "type", "status" etc. without specifying what type, what status or better yet, avoiding those words altogether
* Use ISO standard or other generally used (see above) values for attribute values such as languages, country names etc. Avoid using magic numbers as values or provide also the human language alternative, preferably according to the Accept-Language header in the request

##### Localization
The Accept-header should be used to support localized strings and possible localized logic. All timestamps should be in ISO format which contains timezone information. All dates and clock times with no specific timezone information associated should be informed in UTC +0.

All money values should be informed in specific currency and currency information should be contained in a custom x-companyname-currency header (in both request and response). Currency values should default to some provider or consumer based base currency if no specific currency has been requested.

##### Privacy and Security
Private or confidential data should not be passed in URI, Query or header parameters as they are logged and cached. Security constraints are defined in API Product level, but privacy and security should be considered when splitting requirements to APIS and endpoints, as security schemes are easier to implement on API level than endpoint level or by reflecting authorization in the allowed operations or response payloads.

##### Versioning
Each API consumer needs to know which version of the API they are using and to be able to subscribe and use the version they need. There are mixed opinions about the way the versioning is indicated: whether API version should be included in the URL or in the header.

The common convention is to have the version in the URL of APIs. The reason is to ensure that the browser is able to explore the resources across versions.

In some API management systems, the version does not need to be in the URI nor in the header because each API product has its own version and each API consuming client application is only able to use 1 version of the API at a time. If the same client used multiple versions of the same API at a time, they would need different subscriptions. This versioning strategy works with all clients and is suited for caching and HATEOAS.

When the version number is used it should always be in the URI since not all clients (for example marketing tools) can set headers and using version number as a query parameter might cause slowness as query parameters are not cached. Also, most API management platforms require that the URIs are unique if multiple versions of the same API are deployed at the same time.

The URI should include /vN with the major version (N) as a prefix. Having the letter v in front of the number is important to separate the version number from a resource identifier.

When APIs are upgraded with a breaking change, it may lead to breaking existing products or services using upgraded APIs.

Privacy and security should be considered when splitting requirements to APIs and endpoints, as security schemes are easier to implement on API level than endpoint level or by reflecting authorization in the allowed operations or response payloads.

Examples of breaking changes:
* Renaming fields or resource paths or endpoints
* Changing field type (e.g. from string to a list of strings)
* Changing the structure of payload (removing/renaming/retyping fields)
* Altering HTTP verbs
* Changing response HTTP codes

In case of breaking changes making a new version of the updated API is mandatory.

##### URI Template
`/v{version}/`

Example:
`https://domain.com/v1/apis`

If there is any major breaking update, the new set of APIs is named as v (version number as integer).

##### Namespaces
In any URI, the first noun (which may be singular or plural, depending on the situation) should be considered a "namespace". Namespaces should reflect the customer's perspective on how the product works, not necessarily hierarchy in the company.

Namespace separates different logical APIs from each other, which is useful if you have lots of APIs with different purposes and they may end up using same resource or operation names.

Namespaces in different API management solutions:
* IBM API Connect uses organizations, catalogs and spaces to organize publishing of APIs. These are useful when there are multiple teams in charge of different APIs. Organization and catalog form the namespace of the API and those are always added automatically before version number or anything defined in the OpenAPI document basepath value or path-variable of each operation.
* Azure API management requires you to define a URI template when adding a new operation or by setting it for all operations in the OpenAPI document basepath value (required).

URI Template:
`/{namespace}/{version}`

Example:
`/hardware/v1/`

##### Resources and HTTP Methods
Try to use only one resource level, absolutely avoid using more than two levels to keep the URLs short to allow room for using variables.

URI Template:
`/{namespace}/{version}/{resource}/{resource-id}/{sub-resource}/{sub-resource-id}`

##### Endpoints
Resource endpoints should follow at least View and CRUD (Create, Read, Update, Delete) operations. These should be handled by using the same URI but using different HTTP verbs (POST/GET/PUT/PATCH/DELETE, more details about each verb in https://www.w3.org/Protocols/rfc2616/rfc2616-sec9.html).

Use nouns in the plural as resource names e.g. `/products`.

All used methods and their parameters have to be described in generated documentation endpoint by endpoint.

##### GET (read)
The GET method requests data from the resource and should not produce any side effect. The possible parameters are sent as part of the URL or as query parameters.

E.g `GET /users`
* Return a list of all users

E.g `GET /users?limit=10&skip=30`
* Returns a list containing 10 users after skipping 30 users

##### POST (create, do partial updates)
The POST method requests the server to create a resource in the database. The payload is sent in the request message body.

POST is a non-idempotent operation which means that multiple requests targeted to the same endpoint with the same payload will have a different outcome.

E.g `POST /organizations/:id/managers`
* The first attempt creates a new Manager of Organization identified with :id. (If it did not exist already)

E.g `POST /organizations/:id/managers`
* The second attempt with the same payload fails (because manager already existed) and an error response (4xx, manager already exists) is returned

##### PUT (create and update complete resources)
The PUT method requests the server to update a resource, but it can also create it. The payload is sent in the request message body. Normally it is not possible to create a resource with PUT method, because resources are referenced with :id. In case resource with :id does not exist, a response with 404 Resource not found is sent unless you give a resource name (like file name) in the PUT request. Use POST to create a new resource and POST or PATCH to do partial updates.

PUT is an idempotent operation which means multiple requests with the same payload targeted to the same endpoint will have the same effect and outcome, either successful update or resource not found.

E.g. `PUT /organizations/:id`
* The first attempt will request the server to update the resource (identified with :id) in Organizations collection
* A successful response with 2xx is returned, if a resource is found
* In case the resource is not found, an error response with 4xx is returned

E.g. `PUT /organizations/:id`
* Second attempt (with the same payload) will request the server to update the resource (identified with :id) in Organizations collection
* A successful response to 2xx is returned, if the resource is found
* In case the resource is not found, an error response with 4xx is returned

##### DELETE (delete)
DELETE method requests that the resource, or its instance, should be removed from the database. The operation is irreversible.

E.g `DELETE /apis/:id`
* Will request the server to delete the API identified with :id from Apis collection
* In a successful case a response with 204 is returned (no payload included)
* In an unsuccessful case, a response with 4xx is returned

##### Error Handling
Just like an HTML error page shows a useful error message to a visitor, an API should provide a useful error message in a known consumable format. The representation of an error should be no different from the representation of any resource, just with its own set of fields.

The API should always return sensible HTTP status codes. API errors typically break down into 2 types: 400 series status codes for client issues & 500 series status codes for server issues. At a minimum, the API should standardize that all 400 series errors come with consumable JSON error representation. If possible (i.e. if load balancers & reverse proxies can create custom error bodies), this should extend to 500 series status codes.

A JSON error body should provide a few things for the developer - a useful error message, a unique error code (that can be looked up for more details in the docs) and possibly a detailed description.

JSON output representation for something like this would look like:
```json
{
    "code": 1234,
    "title": "Organization is not found",
    "detail": "Organization with specified ID is not found"
}
```

Validation errors for PUT, PATCH and POST requests will need a field breakdown. This is best modeled by using a fixed top-level error code for validation failures and providing the detailed errors in an additional errors field, like so:
```json
{
    "code": 1024,
    "title": "Validation Failed",
    "detail": [
        {
            "code": 5432,
            "title": "first_name",
            "detail": "First name cannot have fancy characters"
        },
        {
            "code": 5622,
            "title": "password",
            "detail": "Password cannot be blank"
        }
    ]
}
```

##### Filtering

###### Paging
Pages of results should be referred to consistently by the query parameters page and pageSize, where pageSize refers to the number of results per request, and page refers to the requested page.

Fields like totalItems and totalPages help provide context to paged results. Use the same fields with all resources to be consistent.

###### Hypermedia Links
Hypermedia links are high value in navigating paged resource collections, as page/pageSize query parameters can be maintained while navigating pages of results.

Links should be provided with reels of next, previous, first, last wherever appropriate.

###### Time Selection
startTime or {propertyName}After, endTime or {propertyName}Before query parameters should be provided if time selection is needed. All time values in the parameters and in the data have to be in the ISO format including timezone.

###### Sorting
sortBy and sortOrder can be provided to allow for collection results to be sorted. sortBy should be a field in the individual resources, and sortOrder should be asc or desc.

URI Template:
`GET /{namespace}/{version}/{resource}`

Example Request:
`GET /hardware/v1/products`

##### Resource Collection
A list of all of the given resources, including any related metadata. The array of resources should be in the items field to help handle other fields than the actual resources being returned in the response.

Plan for security and provide a list of only those resources the requesting party is allowed to see.

If the resource response is really big, provide a possibility to include only those fields the client requires. Also add only those fields in the response, that you consider absolutely necessary. It's easier to add more later when needed instead of removing that would be a breaking change.

##### Single Resource
A single resource, typically derived from the parent collection of resources (often more detailed than the collection resource items).

All identifiers for sensitive data should be non-sequential, and preferably non-numeric. In scenarios where this data might be used as a subordinate to other data, immutable string identifiers should be utilized for easier readability and debugging (i.e. "nameOfValue" vs 1421321).

URI Template:
`GET /{namespace}/{version}/{resource}/{resource-id}`

Example Request:
`GET /hardware/v1/products/6438313255314`

## API Audit
*For Architects, API Developers, API Product Managers*

The API Audit phase ensures that API designs align with organizational guidelines and best practices. This phase leverages structured checklists to assess key areas, including business requirements, developer experience, compliance with standards, and security considerations.

**Note:** The APIOps Cycles API Audit checklist serves as a foundation for building customized checklists tailored to specific needs. While comprehensive, it does not replace rigorous security assessments or guarantee completely secure APIs.

### Prepare for the Audit
* Collect all API-related documentation from previous stations (e.g., design specs, consumer feedback, performance benchmarks)
* Define the audit's scope (e.g., functional, security, operational)

### Conduct the Audit
Evaluate the API against key criteria:
* Functional: Are all endpoints working as designed? Do they meet the consumer requirements?
* Non-Functional: Is the API scalable, secure, and performant within the defined thresholds?
* Consumer Perspective: Does the API documentation accurately represent the current functionality? Are developer portals and onboarding processes seamless?

Use automated tools where applicable.

### Rest API Checklist

#### Concept is Ready When
* The API is based on clear business needs. (API9:2019 Improper Assets Management)
* API is designed for hiding raw backend data and shared use for multiple API-consuming applications (API6:2023 Excessive Data Exposure)
* The API and its endpoints have a description that explains its business value and features. (API9:2023 Improper Inventory Management)
* API has a consistent design with our other APIs. (API8:2023 Security Misconfiguration, API9:2023 Improper Inventory Management)
* API and data naming of attributes uses good, descriptive English (or other standard language)
* Mandatory fields are specified (API6:2019 Mass Assignment)
* Dates are in ISO standard date format including the timezone. (API8:2019 Injection)
* All general data such as country and language names, geographical coordinates etc. use (ISO or other) standard values. (API6:2023 Excessive Data Exposure, API8:2019 Injection)
* Fields are described in full words avoiding acronyms. (API9:2023 Improper Inventory Management)
* When creating new resources, an identifier is returned per item. (API2:2023 Broken Authentication)

#### API Design Prototype is Ready When
* Endpoint design contains maximum of two resources/sub-resources in the endpoint path
* All endpoints and attributes include examples
* POST is used for creating and updating data (instead of PUT unless full resource)
* DELETE is used to remove a resource
* API versioning strategy has been decided and it is supported by the API gateway in use. (API9:2023 Improper Inventory Management)
* GET method doesn't have a request body and returns status 200 OK and some content in response
* GET method returns status 204 when the response body is empty
* POST method returns 200 OK when the resource is updated
* POST method returns status 201 Created and returns the identifier of the created resource
* DELETE method returns 204 OK when removing a resource was successful
* 400 -responses have additional information on the specific error (for example, missing required attribute but not internal or infrastructure information) (API6:2023 Excessive Data Exposure)
* 401 Unauthorized is used when the API consumer is using the wrong credentials (API2:2023 Broken Authentication)
* 403 Forbidden is used when an authorized API consumer tries to use an operation they are not allowed to do. (API5:2023 Broken Function Level Authorization)

#### API is Maintainable in Production When
* API is published via API management (API10:2019 Insufficient Logging & Monitoring, API8:2023 Security Misconfiguration)
* API is visible in a Developer portal (API9:2023 Improper Inventory Management)
* API can only be accessed via the API management gateway (API9:2023 Improper Inventory Management, API8:2023 Security Misconfiguration)
* Rate limits are enforced when requesting API (API4:2023 Unrestricted Resource Consumption)
* API documentation is generated automatically based on the specification, schema and examples (API9:2023 Improper Inventory Management)
* The specification is updated automatically to API gateway and documentation site / developer portal when changes are done to API (API9:2023 Improper Inventory Management)
* Specification for endpoints is validated on every change against standards
* The specification contains the schema for the requests and responses
* Request and response schema and examples pass schema validation
* API uses HTTPS (or, in special cases, other stateless protocols with encryption) (API10:2023 Unsafe Consumption of APIs)
* The API published under the organization's official domain (API8:2023 Security Misconfiguration)
* All endpoints are protected by authentication (API2:2023 Broken Authentication, API4:2023 Unrestricted Resource Consumption)
* API has token-based authentication
* API is protected against Cross Site Request Forgery (CFRS) (API8:2023 Security Misconfiguration)
* Inputs are validated automatically by the coding framework used (API8:2023 Security Misconfiguration)
* Outputs are escaped automatically by the coding framework used (API8:2023 Security Misconfiguration)
* Encryption of data in transit and data in storage is implemented according to the evaluated need (API8:2023 Security Misconfiguration)
* Message integrity has been implemented according to the evaluated need (API6:2023 Unrestricted Access to Sensitive Business Flows, API7:2023 Server Side Request Forgery)
* UUID or other pseudoidentifiers are used to identify objects instead of internal database identifiers (API7:2023 Insecure Direct Object References)
* Direct object references to sensitive information like bank account numbers, social security numbers, person names are not used in URLs (API7:2023 Insecure Direct Object References)
* Specific HTTP Methods are only available for resources where intended (e.g. whitelisting, automatically based on OpenAPI specification) (API5:2023 Broken Function Level Authorization)

#### Async API Checklist

##### Concept is Ready When
* The API is based on clear business needs
* API is designed for hiding raw backend data and shared use for multiple API-consuming applications
* The API has a description that explains its business value and features
* API has a consistent design with our other APIs
* API and data naming uses good English (or other standard language)
* Mandatory fields are specified
* Dates are in ISO standard date format including the timezone
* All general data such as country and language names, geographical coordinates etc. use standard values
* Fields are described in full words avoiding acronyms
* When publishing new messages, the relevant topics or channels are clearly identified

##### API Design Prototype is Ready When
* The message design contains a clear structure, differentiating between events, commands, and queries
* All messages and attributes include examples
* Messages follow a consistent structure across all topics/channels
* The message versioning strategy has been decided
* Acknowledgments for received messages are defined (if applicable)
* Errors or issues with messages are clearly conveyed, with additional information on the specific error
* Authentication and authorization strategies are specified

##### API is Maintainable in Production When
* API is managed via a proper AsyncAPI management tool
* API is visible in a Developer portal
* Rate limits are enforced when sending messages (if applicable)
* API documentation is generated automatically based on the AsyncAPI specification, schema, and examples
* The specification is updated automatically to API management tools and documentation site/developer portal when changes are done to API
* Specification for topics/channels is validated on every change against standards
* The specification contains the schema for the messages
* Message schema and examples pass schema validation
* Message transport ensures security (e.g., MQTT over TLS or AMQP over TLS)
* The API is operated under the organization's official domain (or relevant broker or message service)
* All topics/channels are protected by authentication
* API has token-based authentication
* Encryption of data in transit and data in storage is implemented according to the evaluated need
* Message integrity has been implemented according to the evaluated need
* UUID or other pseudoidentifiers are used to identify objects instead of internal database identifiers
* Sensitive information is not exposed in topics or channels
* Message integrity has been implemented according to the evaluated need
* UUID or other pseudoidentifiers are used to identify objects instead of internal database identifiers
* Sensitive information is not exposed in topics or channels
* Whitelisting is used to specify which clients can publish or subscribe to certain topics/channels

### Report and Act
* Compile findings into a short report
* Classify issues based on criticality (e.g., must-fix, should-fix, optional enhancements)
* Plan remediation steps, assigning them to relevant teams

## API Publishing
*For Architects, API Developers, API Product Managers*

After auditing the API to ensure it meets functional, security, and performance standards, the next step is to make it accessible and usable for API consumers. API Publishing focuses on providing developers and stakeholders with the tools, documentation, and support they need to successfully integrate the API.

### Prepare Publishing Resources
* Finalize API documentation, including examples, tutorials, and technical specifications
* Set up the API in a developer portal with onboarding instructions, authentication details, and sandbox environments

### Enable API Accessibility
* Decide on the publishing scope: private (internal teams), partner (trusted collaborators), or public (broad audience)
* Provide clear registration and access mechanisms for API consumers (e.g., API keys, OAuth)
* Ensure APIs are easy to integrate into target systems

### Support API Consumers
* Offer real-time support through forums, ticketing systems, or chat
* Use feedback tools to capture insights on consumer needs and potential issues
* Monitor API usage (e.g., traffic, error rates, latency) and ensure SLA commitments are met

## API Adoption
*For API Product Managers, Business Leaders*

API Adoption is where your published API begins to make an impact. This phase ensures your API is integrated into the daily workflows of your consumers, whether they are developers, applications, or systems. Success here is not only about the number of integrations but how effectively your API solves consumer problems and delivers value.

### Onboarding API Consumers
Create a seamless experience for API consumers to start using your API:
* Provide detailed, intuitive documentation
* Set up a sandbox environment for testing and experimentation
* Offer starter kits, sample integrations, and code snippets
* Ensure clear error messages and troubleshooting guides
* Set up support channels: Developer forums, chat support, or dedicated onboarding sessions

To check: Are there blockers in the onboarding process that could frustrate developers?

### Tracking and Measuring Adoption
Use data to understand how your API is being used:

Engagement Metrics:
* Number of registered API consumers
* Frequency and volume of API calls by endpoint

Consumer Experience Metrics:
* Time to first successful API call (TTF)
* Error rates and retry patterns
* Latency and response times

Satisfaction Metrics:
* Developer Net Promoter Score (NPS)
* Feedback on documentation and usability
* Use monitoring tools like Postman Analytics, Datadog, or Apigee to visualize adoption and identify gaps

To check: Are the API usage patterns aligned with consumer needs and expectations?

### Iterating and Improving
Use insights from metrics and consumer feedback to:
* Address pain points in documentation, onboarding, or performance
* Add missing features or optimize API functionality
* Improve error handling with clearer error codes and retry strategies
* Collaborate with teams responsible for publishing and platform architecture to implement improvements

To check: Are we closing the loop between consumer feedback and API enhancements?