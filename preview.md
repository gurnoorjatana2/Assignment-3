# Assignment: Architectural Decision Records

## ADR: Development Approach for University Social Networking App

*Decision Title:* Choosing Between Native, Web, or Hybrid Development

*Context:* To reach both iOS and Android users in the university community, we need an efficient development approach that supports widespread accessibility.

*Decision:* The decision is made to use a hybrid development approach with React Native.

*Rationale:*
- *Broad Reach:* Hybrid apps can be deployed on both iOS and Android from a single codebase.
- *Development Efficiency:* Allows for sharing code across platforms, speeding up development and simplifying maintenance.
- *Community and Resources:* React Native has a large developer community, providing access to a wealth of resources and support.

*Consequences:*
- *Performance Considerations:* While React Native approaches native performance, there may be cases where optimization is needed for intensive tasks.
- *Learning Curve:* Developers unfamiliar with React Native or JavaScript may need training.

*Follow-Up Actions:*
- Plan training for developers new to React Native.
- Optimize performance for both platforms, focusing on intensive features.

## ADR: UI Framework Selection for University Social Networking App

*Decision Title:* UI Framework for Hybrid Development

*Context:* A compelling and user-friendly UI is crucial for engaging students and professors with the app.

*Decision:* React Native will be used for the UI, leveraging its component-based framework to create a seamless experience on both iOS and Android.

*Rationale:*
- *Consistency Across Platforms:* Ensures a unified look and feel.
- *Component Rich:* Offers a wide array of pre-built and customizable components.
- *Performance:* React Native's components are optimized for mobile devices, ensuring smooth interactions.

*Consequences:*
- *Design Flexibility:* May need creative solutions for highly custom designs outside the standard component library.
- *Upkeep:* Staying updated with the latest React Native versions is necessary to leverage new UI components and features.

*Follow-Up Actions:*
- Utilize React Native's UI components to design intuitive interfaces.
- Regularly update skills and knowledge to incorporate new React Native features.

## ADR: Backend Language for University Social Networking App

*Decision Title:* Selection of Backend Language

*Context:* The backend must efficiently handle data processing, authentication, and integration with university systems.

*Decision:* Node.js is selected as the backend language.

*Rationale:*
- *Scalability:* Handles concurrent requests efficiently, crucial for real-time features.
- *Ecosystem:* A vast npm ecosystem offers libraries and tools for rapid development.
- *Integration:* Facilitates easy integration with databases, Active Directory, and other APIs.

*Consequences:*
- *Skillset Requirements:* Requires JavaScript proficiency among backend developers.
- *Resource Management:* Effective handling of CPU-intensive tasks is necessary to avoid performance bottlenecks.

*Follow-Up Actions:*
- Ensure the development team is proficient in Node.js and asynchronous programming patterns.
- Implement best practices for resource management and optimization.

## ADR: Permissions Management in University Social Networking App

*Decision Title:* Implementing Permissions for Data Access and Functionality

*Context:* Proper permissions management is essential for securing sensitive information and ensuring users only access features relevant to their roles.

*Decision:* Implement dynamic permissions management, integrating with the university's Active Directory for authentication and role-based access control.

*Rationale:*
- *Security and Privacy:* Ensures that user data is protected and access is appropriately restricted.
- *Role-Based Access:* Differentiates features and data access between students and professors.
- *Compliance:* Meets legal and institutional requirements for data handling and privacy.

*Consequences:*
- *Implementation Complexity:* Requires careful planning to map and enforce permissions accurately.
- *Maintenance:* Roles and permissions may need updates to reflect changes in app features or university policies.

*Follow-Up Actions:*
- Design a comprehensive role and permissions matrix in collaboration with university stakeholders.
- Develop and test integration with Active Directory to manage user authentication and authorization.

## ADR: Data Storage Strategy for University Social Networking App

*Decision Title:* Approach to Storing and Accessing App Data

*Context:* The app needs a reliable data storage solution to support offline access and efficient data synchronization.

*Decision:* A hybrid data storage approach using both local storage (for offline access) and cloud storage (for data synchronization and backup).

*Rationale:*
- *Offline Accessibility:* Allows users to access important information without an internet connection.
- *Data Sync:* Ensures user data is up-to-date across devices.
- *Scalability:* Cloud storage can scale with the app’s user base and data needs.

*Consequences:*
- *Complexity in Syncing:* Managing data consistency between local and cloud storage requires robust syncing mechanisms.
- *Data Management:* Must ensure data stored on devices is secure and does not overly consume device storage.

*Follow-Up Actions:*
- Implement data encryption for local storage to enhance security.
- Develop a syncing mechanism that minimizes data usage and ensures up-to-date information.

## ADR: Integrating Additional Frameworks and Technology Stacks

*Decision Title:* Adoption of Additional Technologies for Enhanced Functionality

*Context:* To enrich the app with modern features such as push notifications, real-time updates, and secure data handling, integrating with additional frameworks and technology stacks is considered.

*Decision:* Incorporate Firebase for real-time database, authentication, and push notifications, along with other selected APIs and frameworks for specific functionalities.

*Rationale:*
- *Feature-Rich:* Firebase offers a suite of services that are ideal for building dynamic, interactive apps.
- *Scalability:* Easily scales to accommodate a growing number of users.
- *Security:* Provides robust security features to protect sensitive data.

*Consequences:*
- *Vendor Lock-In:* Reliance on Firebase and other third-party services may limit future flexibility.
- *Learning Curve:* The development team may need to familiarize themselves with Firebase and other new technologies.

*Follow-Up Actions:*
- Provide training sessions on Firebase and other technologies to be used.
- Evaluate and plan for potential risks associated with vendor lock-in, including contingency strategies for critical services.
