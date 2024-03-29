# Choosing Layered Architecture for C# REST API and NEXT.JS Frontend

## Status 
- Accepted

## Context and Problem Statement 
Determining the appropriate architectural design approach for both the backend (C#) and the frontend (NEXT.JS), proved to be a difficult decision. The goal was to ensure that the code was maintainable, scalable and used separation of concerns throughout the application. 

## Considered Options
- _Layered Architecture_: Separating the application into distinct layers (presentation, business and data access)
- _Component-Based Architecture_: System structured into self-contained modular units called components and each one encapsulates a set of functionalities.
- _Microservices Architecture_: Decomposed the system into small, independent deployable services.
  
## Decision Outcome 
_Chosen option_: "Layered Architecture" was adopted for both the C# REST API (Backend) and NEXT.JS (Frontend). This is due to the fact that Layered Architecture provides separation of concerns, making it easier to update and adapt specific components of the system without affecting others. This flexibility makes testing and future deployments much easier to do since each layer is only responsible for a specific task. 

While there are many benefits with Component-Based Architecture, for the nature of the system Layered was considered an ideal choice due the complex business logic that would be occurring within multiple components, making dependency management more difficult. 

## Consequences
While Layered Architecture offers many advantages, setting up the initial structure of the application required more effort that I originally thought. It was difficult to understand each components within the C4 diagram as I constantly got the layers wrong and had to change the diagram several times. However, once the style was correct - it was easy to understand how each component would react to each other within the code. 

## More information 
- https://bitloops.com/docs/bitloops-language/learning/software-architecture/layered-architecture
- https://medium.com/geekculture/what-is-a-layered-architecture-in-software-design-22152fc06822
