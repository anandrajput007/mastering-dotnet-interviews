# Mastering .NET Interviews 🚀

This repository contains curated **.NET interview questions and concise answers**
covering C#, .NET Core, LINQ, Entity Framework, Microservices, Design Patterns,
SQL, Multithreading, and System Design.

The goal is to build strong conceptual clarity for **Mid-Level, Senior, and Architect-level interviews**.

---

## 📚 Topics Covered

1. C# Fundamentals & Advanced  
2. .NET Core & ASP.NET Core  
3. LINQ  
4. Entity Framework  
5. Microservices  
6. Design Patterns  
7. SOLID Principles  
8. Multithreading & Async/Await  
9. SQL & Performance  
10. System Design (Senior Level)

---

## C# Fundamentals & Advanced

1. What is the difference between IEnumerable and IQueryable?
- `IEnumerable` executes queries in memory.
- `IQueryable` translates queries to a data source (like SQL) and executes remotely.

2. How does async/await work internally?
- The compiler converts async methods into a state machine.
- Execution pauses at `await` and resumes when the awaited task completes.

3. What is the difference between abstract class and interface?
- Abstract class can contain implementation and state.
- Interface defines a contract (supports default methods in newer versions).

---

## .NET Core & ASP.NET Core

1. What is Middleware?
- Middleware forms the HTTP request pipeline.
- Order of registration determines execution sequence.

2. Explain Dependency Injection lifetimes.
- **Transient** – New instance every time.
- **Scoped** – One instance per HTTP request.
- **Singleton** – One instance for application lifetime.

3. What makes .NET Core different from .NET Framework?
- Cross-platform support.
- Lightweight and modular.
- Better suited for cloud and microservices.

---

## LINQ

1. What is Deferred Execution?
- Query executes only when enumerated (e.g., `foreach`).
- Methods like `ToList()` trigger immediate execution.

2. Difference between First and Single?
- `First` returns first matching element.
- `Single` ensures exactly one match and throws if multiple exist.

3. What are projection and filtering operators?
- Projection → `Select()`
- Filtering → `Where()`

---

## Entity Framework

1. What is Change Tracking?
- EF Core tracks entity states (Added, Modified, Deleted).
- Automatically generates appropriate SQL during `SaveChanges()`.

2. Explain Eager, Lazy, and Explicit Loading.
- **Eager Loading** – `Include()` loads related data immediately.
- **Lazy Loading** – Data loads when accessed.
- **Explicit Loading** – Manually loaded using context.

3. What is AsNoTracking()?
- Disables change tracking.
- Improves read-only query performance.

---

## Microservices

1. What are key characteristics of microservices?
- Independent deployment.
- Bounded context.
- Decentralized data management.

2. How do microservices communicate?
- REST APIs
- gRPC
- Message brokers (RabbitMQ, Kafka)

3. What is an API Gateway?
- Single entry point for client requests.
- Handles routing, authentication, rate limiting, aggregation.

---

## Design Patterns

1. What is the Singleton pattern?
- Ensures only one instance exists throughout application lifetime.

2. What is the Factory pattern?
- Encapsulates object creation logic.

3. What is the Repository pattern?
- Separates data access logic from business logic.

---

## SOLID Principles

1. What is Single Responsibility Principle?
- A class should have only one reason to change.

2. What is Open/Closed Principle?
- Open for extension, closed for modification.

3. What is Dependency Inversion Principle?
- Depend on abstractions, not concrete implementations.

---

## Multithreading & Async/Await

1. What is the difference between Thread and Task?
- Thread is OS-level construct.
- Task is managed by .NET ThreadPool.

2. What is a deadlock?
- Two threads wait indefinitely for each other’s resources.

3. What is ConfigureAwait(false)?
- Prevents capturing synchronization context.
- Improves performance in library code.

---

## SQL & Performance

1. What is indexing?
- Improves query speed by reducing full table scans.

2. Difference between Clustered and Non-Clustered Index?
- Clustered → Defines physical order of data.
- Non-Clustered → Separate structure referencing data.

3. How do you optimize slow queries?
- Analyze execution plans.
- Use proper indexing.
- Avoid SELECT *.
- Optimize joins.

---

## System Design (Senior Level)

1. How would you design a scalable Web API?
- Stateless services.
- Load balancing.
- Caching.
- Horizontal scaling.

2. What caching strategies can be used?
- In-memory caching.
- Distributed caching (Redis).
- Response caching.

3. How do you handle high traffic systems?
- Auto-scaling.
- Rate limiting.
- CDN usage.
- Asynchronous processing.

---

## 🎯 Target Audience

- Mid-Level Developers
- Senior Developers
- Tech Leads
- Architects
