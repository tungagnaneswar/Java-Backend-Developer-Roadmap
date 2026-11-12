# Java Backend Interview Roadmap

> Target: Java Full Stack / Backend roles (1.5 to 3 years experience)
> How to use: tick `[x]` as you finish each topic. Do the phases in order. Run **DSA daily in parallel** (see Track B).

**Legend**
- 🔴 Must know (asked in almost every interview)
- 🟡 Important (asked often)
- 🟢 Good to have (bonus / senior-leaning)
- 🆕 Added gap, not in your original list

---

## Overall Plan

| Phase | Focus | Priority | Suggested time |
|---|---|---|---|
| 1 | Core Java + OOP | 🔴 | 2 weeks |
| 2 | Collections + Exceptions | 🔴 | 1.5 weeks |
| 3 | Java 8+ (Lambda, Streams, Optional) | 🔴 | 1 week |
| 4 | Multithreading + Concurrency | 🔴 | 1.5 weeks |
| 5 | SQL + JDBC | 🔴 | 1.5 weeks |
| 6 | JPA / Hibernate / Spring Data JPA | 🔴 | 1.5 weeks |
| 7 | Spring Core + Spring Boot + MVC | 🔴 | 2 weeks |
| 8 | Spring Security + JWT | 🔴 | 1 week |
| 9 | HTTP / REST / Networking | 🟡 | 1 week |
| 10 | 🆕 Testing (JUnit 5 + Mockito) | 🔴 | 1 week |
| 11 | JVM + Memory | 🟡 | 1 week |
| 12 | Redis / Caching | 🟡 | 1 week |
| 13 | Kafka / Messaging | 🟡 | 1 week |
| 14 | 🆕 Microservices + System Design | 🟡 | 2 weeks |
| 15 | JavaScript, React, TypeScript (revision) | 🟡 | 1 week |
| 16 | 🆕 Design Patterns + SOLID | 🟡 | 1 week |
| 17 | 🆕 Docker, CI/CD, AWS, Git (revision) | 🟡 | 3 to 4 days |
| 18 | AI / LLM | 🟢 | 1 week |

Total is roughly 4 months at 1.5 to 2 hours a day. Do not skip Phases 1 to 10; they decide most interviews.

---

# TRACK A: Topic Phases

## Phase 1: Core Java + OOP 🔴

**OOP**
- [ ] Class, Object
- [ ] Encapsulation, Inheritance, Polymorphism, Abstraction
- [ ] Composition vs Inheritance

**Java Basics**
- [ ] Primitive vs Wrapper classes, Autoboxing / Unboxing
- [ ] `static`, `this`, `super`
- [ ] Constructor, Constructor chaining
- [ ] Access modifiers (public, private, protected, default)
- [ ] `final`, `final` vs `finally` vs `finalize`
- [ ] Object class, Enum
- [ ] Pass-by-value in Java
- [ ] 🆕 String, String Pool, StringBuilder vs StringBuffer, why String is immutable
- [ ] 🆕 Java 17 / 21 features: records, sealed classes, switch expressions, text blocks, `var`

**Methods**
- [ ] Overloading, Overriding, Varargs

**Interfaces & Classes**
- [ ] Interface, Abstract class, Interface vs Abstract class
- [ ] Default methods, Static methods in interfaces

**Object & Memory Concepts**
- [ ] `==` vs `equals()`, `hashCode()`
- [ ] Immutable class (how to create one)
- [ ] Shallow vs Deep copy, `clone()` basics

**Nested Types**
- [ ] Inner classes, Static nested classes, Anonymous classes

**Generics**
- [ ] Generic classes, Generic methods
- [ ] `<T>`, `<?>`, `<? extends T>`, `<? super T>` (PECS rule)

**Control Constructs** (quick revision only)
- [ ] if-else, loops, switch-case, break, continue, labeled statements

---

## Phase 2: Collections + Exceptions 🔴

**Collections**
- [ ] Hierarchy: Collection vs Collections, Iterable, List, Set, Queue, Map
- [ ] List: ArrayList, LinkedList, Vector
- [ ] Set: HashSet, LinkedHashSet, TreeSet
- [ ] Map: HashMap, LinkedHashMap, TreeMap, Hashtable, ConcurrentHashMap
- [ ] Queue: PriorityQueue, Deque, ArrayDeque

**Important Concepts (very frequently asked)**
- [ ] Hashing, `hashCode()` and `equals()` contract
- [ ] HashMap internal working (buckets, treeification at 8)
- [ ] HashSet internal working
- [ ] Collision, Load factor, Initial capacity, Resize / Rehashing
- [ ] Comparable vs Comparator, `Collections.sort()`, Custom sorting
- [ ] 🆕 Fail-fast vs Fail-safe iterators, `ConcurrentModificationException`
- [ ] 🆕 HashMap vs ConcurrentHashMap vs Hashtable vs `Collections.synchronizedMap`

**Exception Handling**
- [ ] Exception hierarchy, Checked vs Unchecked
- [ ] try, catch, finally, throw, throws
- [ ] Custom exceptions, Multiple catch
- [ ] Try-with-resources
- [ ] Exception propagation
- [ ] Best practices

---

## Phase 3: Java 8+ 🔴

- [ ] Lambda expressions
- [ ] Functional interfaces: Predicate, Function, Consumer, Supplier (+ 🆕 BiFunction, UnaryOperator)
- [ ] Method references
- [ ] Default and static interface methods

**Stream API**
- [ ] `stream()`, `map()`, `filter()`, `flatMap()`, `reduce()`
- [ ] `sorted()`, `distinct()`, `limit()`, `skip()`, `count()`
- [ ] `anyMatch()`, `allMatch()`, `noneMatch()`, `findFirst()`, `findAny()`
- [ ] Collectors: `groupingBy()`, `partitioningBy()`, `joining()`, 🆕 `toMap()`, `counting()`
- [ ] 🆕 Parallel streams (when NOT to use them)
- [ ] Optional

> **Practice:** solve 20 stream coding questions (group employees by department, highest salary per dept, word frequency, second highest number).

---

## Phase 4: Multithreading + Concurrency 🔴

**Basics**
- [ ] Process vs Thread, Thread lifecycle
- [ ] Thread class, Runnable, Callable

**Thread Control**
- [ ] `start()` vs `run()`, `sleep()`, `join()`
- [ ] `wait()`, `notify()`, `notifyAll()`

**Synchronization**
- [ ] `synchronized`, `volatile`, Atomic classes
- [ ] Lock, ReentrantLock

**Concurrency**
- [ ] ExecutorService, ThreadPool, Future
- [ ] 🆕 CompletableFuture (you used parallel Promises in Node; know the Java equivalent)
- [ ] Concurrent collections
- [ ] 🆕 `@Async` in Spring, ThreadLocal basics

**Problems & Concepts**
- [ ] Race condition, Deadlock, Starvation
- [ ] Thread safety, Mutual exclusion
- [ ] Executor vs manual Thread creation
- [ ] 🆕 Write: producer-consumer, deadlock example, thread-safe singleton

---

## Phase 5: SQL + JDBC 🔴

**SQL Basics**
- [ ] SELECT, WHERE, DISTINCT, ORDER BY, GROUP BY, HAVING, LIMIT / OFFSET, CASE

**Joins**
- [ ] INNER, LEFT, RIGHT, FULL, CROSS, Self join

**Queries**
- [ ] Subqueries, EXISTS, IN, UNION vs UNION ALL, CTE
- [ ] 🆕 Window functions: `ROW_NUMBER`, `RANK`, `DENSE_RANK`, `LAG`, `LEAD`

**Database Concepts**
- [ ] Primary / Foreign / Unique / Composite keys, Constraints
- [ ] Normalization, Denormalization, Views
- [ ] DDL, DML, DCL, TCL
- [ ] Aggregate, String, Date, Numeric, User-defined functions
- [ ] Triggers

**Database Features**
- [ ] Transactions, ACID, Isolation levels
- [ ] Indexes, Composite indexes, Clustered vs non-clustered
- [ ] EXPLAIN / query execution plan, Query optimization

**JDBC** (lighter, asked less than JPA)
- [ ] Architecture, Driver, Connection
- [ ] Statement, PreparedStatement, CallableStatement
- [ ] ResultSet and types
- [ ] commit(), rollback(), Connection pooling (HikariCP)
- [ ] SQL injection, PreparedStatement vs Statement

> **Practice:** Nth highest salary, duplicate rows, employees earning more than manager, top N per group.

---

## Phase 6: Hibernate / JPA / Spring Data JPA 🔴

**JPA**
- [ ] Entity, Entity lifecycle
- [ ] Persistence Context, First-level cache
- [ ] Transactions, 🆕 `@Transactional` (propagation, isolation, rollback rules, self-invocation problem)
- [ ] JPQL, Native queries

**Relationships**
- [ ] `@OneToOne`, `@OneToMany`, `@ManyToOne`, `@ManyToMany`
- [ ] `mappedBy`, Owning side, Cascade, `orphanRemoval`

**Fetching**
- [ ] Lazy vs Eager loading
- [ ] **N+1 problem** and fixes (`JOIN FETCH`, Entity Graph)
- [ ] 🆕 `LazyInitializationException`

**Hibernate**
- [ ] Architecture, Session, SessionFactory
- [ ] Dirty checking, HQL
- [ ] 🆕 Second-level cache (basics)

**Spring Data JPA**
- [ ] Repository, CrudRepository, JpaRepository
- [ ] Derived query methods, `@Query`
- [ ] Pagination, Sorting
- [ ] 🆕 Projections, `@Modifying`

**Important Comparisons**
- [ ] JPA vs Hibernate vs Spring Data JPA
- [ ] Optimistic locking (`@Version`) vs Pessimistic locking
- [ ] 🆕 Database migrations: Flyway / Liquibase

---

## Phase 7: Spring Core + Spring Boot + Spring MVC 🔴

**Spring Core**
- [ ] IoC, Dependency Injection (Constructor, Setter, Field), why constructor injection is preferred
- [ ] Bean, Bean lifecycle, Bean scopes
- [ ] Component scanning, ApplicationContext
- [ ] `@Component`, `@Service`, `@Repository`, `@Controller`, `@Autowired`, `@Configuration`, `@Bean`
- [ ] 🆕 `@Qualifier`, `@Primary`, circular dependency
- [ ] 🆕 AOP basics (how `@Transactional` works through proxies)

**Spring Boot**
- [ ] Spring Boot vs Spring Framework
- [ ] Starter dependencies, Auto-configuration (how it works)
- [ ] `application.properties` / `.yml`, Profiles
- [ ] Configuration properties, Environment variables
- [ ] Actuator, Logging

**REST in Spring**
- [ ] `@RestController`, `@RequestMapping`, `@GetMapping`, `@PostMapping`, `@PutMapping`, `@PatchMapping`, `@DeleteMapping`
- [ ] `@RequestParam`, `@PathVariable`, `@RequestBody`, `@ResponseBody`, `ResponseEntity`

**Architecture**
- [ ] Controller → Service → Repository, DTO vs Entity, Mapper (MapStruct)

**Validation**
- [ ] `@Valid`, `@NotNull`, `@NotBlank`, `@Size`, `@Email`, Custom validation

**Exception Handling**
- [ ] `@ExceptionHandler`, `@ControllerAdvice`, `@RestControllerAdvice`, Global handling

**Spring MVC**
- [ ] Architecture, DispatcherServlet, Handler Mapping
- [ ] Request processing flow, Message converters
- [ ] 🆕 Interceptors vs Filters

**Servlets (revision only)**
- [ ] Servlet, Lifecycle, Container, doGet / doPost
- [ ] Session, Cookies, Filters
- [ ] Servlet vs Spring MVC

---

## Phase 8: Spring Security + JWT 🔴

- [ ] Authentication vs Authorization
- [ ] AuthenticationManager, SecurityContext, SecurityContextHolder
- [ ] SecurityFilterChain, Security filters (filter order)
- [ ] Roles vs Authorities, RBAC, Access control
- [ ] Password hashing, BCrypt, PasswordEncoder
- [ ] JWT structure, Access token, Refresh token, full JWT flow
- [ ] CORS, CSRF, CORS vs CSRF
- [ ] 🆕 Method-level security (`@PreAuthorize`)
- [ ] 🆕 OAuth2 basics (Authorization Code flow, "Login with Google")

> **Be ready to draw:** the full login → JWT → request filter → SecurityContext flow from your own project.

---

## Phase 9: HTTP / REST / Networking 🟡

**HTTP**
- [ ] Request / Response, Headers, Body
- [ ] Content-Type, Accept, Authorization
- [ ] Cookies, Sessions

**Methods and Status Codes**
- [ ] GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD
- [ ] 2xx, 3xx, 4xx, 5xx: 200, 201, 204, 400, 401, 403, 404, 409, 422, 500, 502, 503
- [ ] 401 vs 403, PUT vs PATCH

**REST**
- [ ] REST principles, Statelessness, Resource-based URLs
- [ ] Idempotency (which methods are idempotent)
- [ ] API versioning, Pagination, Filtering, Sorting
- [ ] 🆕 OpenAPI / Swagger

**Networking**
- [ ] Client vs Server, DNS, IP, Port
- [ ] TCP vs UDP, TCP 3-way handshake
- [ ] HTTPS, TLS/SSL basics
- [ ] Forward Proxy vs Reverse Proxy
- [ ] Load Balancer: Round Robin, Weighted Round Robin, Least Connections, IP Hash
- [ ] CORS, Cookies, Sessions, JWT
- [ ] 🆕 HTTP/1.1 vs HTTP/2, "What happens when you type a URL in the browser?"

---

## Phase 10: 🆕 Testing (JUnit 5 + Mockito) 🔴

*This is a confirmed gap, and now it is on your resume, so interviewers will ask.*

- [ ] Unit test vs Integration test, Test pyramid
- [ ] JUnit 5: `@Test`, `@BeforeEach`, `@AfterEach`, `@ParameterizedTest`, assertions, `assertThrows`
- [ ] Mockito: `@Mock`, `@InjectMocks`, `when().thenReturn()`, `verify()`, `ArgumentCaptor`
- [ ] Spring Boot testing: `@SpringBootTest`, `@WebMvcTest`, `@DataJpaTest`, `MockMvc`
- [ ] Testcontainers (basics)
- [ ] TDD idea, Code coverage (JaCoCo)

> **Practice:** write tests for the service layer of one of your own projects (mock repository, test happy path and exceptions).

---

## Phase 11: JVM + Memory 🟡

- [ ] JVM, JDK vs JRE vs JVM
- [ ] Class Loader
- [ ] Runtime Data Areas: Stack, Heap, Method Area / Metaspace
- [ ] Garbage Collection basics, GC types (G1, ZGC overview)
- [ ] Strong, Weak (🆕 Soft, Phantom) references
- [ ] StackOverflowError, OutOfMemoryError
- [ ] 🆕 Memory leaks: common causes and how to find them (heap dump)
- [ ] 🆕 JVM tuning flags: `-Xms`, `-Xmx`

---

## Phase 12: Redis / Caching 🟡

- [ ] What and why caching
- [ ] Redis, Key-value storage, Data types
- [ ] TTL, Cache hit / miss
- [ ] Cache-aside pattern (+ 🆕 write-through, write-back)
- [ ] Cache invalidation, Eviction policies (LRU, LFU)
- [ ] Redis vs Database
- [ ] 🆕 Spring Cache: `@Cacheable`, `@CacheEvict`, `@CachePut`
- [ ] 🆕 Cache stampede, Cache penetration

> **Hands-on:** run Redis in Docker locally and cache one API response.

---

## Phase 13: Kafka / Message Queues 🟡

**Concepts**
- [ ] Producer, Consumer, Message, Queue, Topic

**Kafka**
- [ ] Broker, Topic, Partition, Consumer Group, Offset
- [ ] Replication, Ordering, Retention
- [ ] 🆕 Delivery guarantees: at-most-once, at-least-once, exactly-once
- [ ] 🆕 Dead Letter Queue, retry
- [ ] 🆕 Spring Kafka: `KafkaTemplate`, `@KafkaListener`

**RabbitMQ**
- [ ] Producer, Consumer, Queue, Exchange, Routing Key

- [ ] Kafka vs RabbitMQ

> **Hands-on:** run Kafka in Docker, produce an event from one Spring Boot app and consume in another.

---

## Phase 14: 🆕 Microservices + System Design 🟡

**Microservices**
- [ ] Monolith vs Microservices
- [ ] Service discovery (Eureka), API Gateway (Spring Cloud Gateway)
- [ ] Inter-service communication: REST, Feign / WebClient, async via Kafka
- [ ] Config server
- [ ] Circuit Breaker (Resilience4j), Retry, Timeout
- [ ] Saga pattern, Database per service
- [ ] Distributed tracing, centralized logging
- [ ] Event-driven architecture, Outbox pattern basics

**System Design Fundamentals**
- [ ] Client → Server, REST API architecture
- [ ] Reverse / Forward proxy, Load balancer
- [ ] Horizontal vs Vertical scaling
- [ ] Caching, Database scaling, Replication, Sharding
- [ ] SQL vs NoSQL, CAP theorem, Consistency, Availability
- [ ] Message Queues, API Gateway, Rate Limiting
- [ ] Authentication, Authorization
- [ ] Logging, Monitoring
- [ ] Retry, Timeout, Circuit Breaker, Idempotency

**Practice Designs**
- [ ] URL Shortener
- [ ] E-commerce Order System
- [ ] Notification System
- [ ] 🆕 Rate Limiter
- [ ] 🆕 Chat / Fleet tracking system (matches your FleetLogix experience)

**Reference architecture**

```
Client
  ↓
Load Balancer
  ↓
API Gateway
  ↓
Spring Boot Services ──→ Redis ──→ Database
  ↓
Kafka
  ↓
Other Services
```

---

## Phase 15: JavaScript, React, TypeScript (revision) 🟡

You work with these daily, so this is mostly sharpening for interview wording.

**JavaScript**
- [ ] `var` / `let` / `const`, Primitive vs Reference types
- [ ] Scope, Hoisting, Closures, `this`
- [ ] Functions, Arrow functions
- [ ] `map()`, `filter()`, `reduce()`
- [ ] Promises, `async` / `await`, `Promise.all` (🆕 vs `allSettled`, `race`)
- [ ] Event Loop (microtasks vs macrotasks)
- [ ] Fetch API, DOM basics
- [ ] 🆕 Node.js + Express: middleware, event loop, error handling (you have this in office projects)

**React**
- [ ] Components, Props, State, Conditional rendering
- [ ] Event handling, Forms, Controlled components
- [ ] API integration, Component lifecycle
- [ ] Hooks: `useState`, `useEffect`, `useContext`, `useCallback`, `useMemo`, `useRef`
- [ ] 🆕 Virtual DOM, keys, re-render causes

**TypeScript**
- [ ] Types, Interfaces, Type aliases
- [ ] Union types, Optional properties
- [ ] Generics, Enums, Type narrowing
- [ ] Basic utility types: `Partial`, `Pick`, `Omit`, `Record`

---

## Phase 16: 🆕 Design Patterns + SOLID 🟡

- [ ] SOLID principles (with a Java example for each)
- [ ] Singleton (thread-safe), Factory, Builder
- [ ] Strategy, Observer, Decorator
- [ ] Where Spring uses them (Singleton beans, Proxy for AOP, Template for JdbcTemplate)
- [ ] 🟢 Low-level design: Parking Lot, Library Management

---

## Phase 17: 🆕 DevOps Basics (revision of your resume skills) 🟡

- [ ] Git: merge vs rebase, resolve conflicts, cherry-pick, branching strategy
- [ ] Docker: Dockerfile, image vs container, volumes, networks, Docker Compose
- [ ] GitHub Actions: build, test, deploy pipeline
- [ ] AWS: S3, EC2 basics, IAM basics
- [ ] Maven / Gradle basics

---

## Phase 18: AI / LLM 🟢

**AI Basics**
- [ ] AI vs ML vs Deep Learning
- [ ] LLM, Tokens, Context window
- [ ] Prompting, Temperature, Embeddings

**LLM Applications**
- [ ] OpenAI API integration, Chatbot, Conversation history
- [ ] Function / Tool calling
- [ ] RAG, Vector database, Semantic search
- [ ] AI Agents, MCP

**Java Integration**
- [ ] Calling LLM APIs from Spring Boot (🆕 Spring AI)
- [ ] Handling responses, Error handling
- [ ] Authentication / API keys (never hardcode, use env variables)

---

# TRACK B: DSA (run daily, 45 to 60 min, alongside every phase)

Do not wait to "finish theory first". Start in Week 1.

**Stage 1 (Weeks 1 to 4)**
- [ ] Big-O: time and space complexity
- [ ] Arrays: traversal, linear search, binary search, two pointers, sliding window
- [ ] Strings: character frequency, anagrams, palindrome, duplicate characters
- [ ] HashMap / HashSet: frequency counting, duplicate detection, Two Sum

**Stage 2 (Weeks 5 to 8)**
- [ ] Sorting: Bubble, Selection, Insertion, Merge, Quick
- [ ] Stack: parentheses, Next Greater Element
- [ ] Queue: basic queue, Deque, Priority Queue
- [ ] Linked List: singly, doubly, reverse, detect cycle, find middle, merge lists

**Stage 3 (Weeks 9 to 16)**
- [ ] Recursion and backtracking basics
- [ ] Trees, Binary Search Tree (traversals, height, LCA)
- [ ] Heap
- [ ] Graph basics (BFS, DFS)
- [ ] 🆕 Basic Dynamic Programming (Fibonacci, climbing stairs, knapsack idea)

**Target:** 100 to 150 problems total (mostly Easy and Medium). Quality over quantity: after each problem, write the pattern name (e.g. "sliding window").

---

# TRACK C: Interview Skills (do not skip)

- [ ] **Project story** for each: FleetLogix, Warehouse Management System, Preserve PMS. For each, prepare: problem, your role, architecture, hardest bug, what you improved, numbers
- [ ] Prepare the FleetLogix report API fix (sequential awaits to parallel, about 60 s down to milliseconds) as a 2-minute story
- [ ] 30-second and 2-minute "Tell me about yourself"
- [ ] Common behavioural answers: conflict, deadline, failure, why switch
- [ ] Mock interviews: at least 3 (friend, or practice speaking answers out loud)
- [ ] Explain every skill on your resume. Remove anything you cannot defend for 10 minutes

---

# Progress Tracker

| Phase | Started | Finished | Confidence (1 to 5) |
|---|---|---|---|
| 1. Core Java + OOP | | | |
| 2. Collections + Exceptions | | | |
| 3. Java 8+ | | | |
| 4. Multithreading | | | |
| 5. SQL + JDBC | | | |
| 6. JPA / Hibernate | | | |
| 7. Spring Core / Boot / MVC | | | |
| 8. Spring Security + JWT | | | |
| 9. HTTP / REST / Networking | | | |
| 10. Testing | | | |
| 11. JVM | | | |
| 12. Redis | | | |
| 13. Kafka | | | |
| 14. Microservices + System Design | | | |
| 15. JS / React / TS | | | |
| 16. Design Patterns | | | |
| 17. DevOps basics | | | |
| 18. AI / LLM | | | |

---

# Weekly Routine (suggestion)

- **Mon to Fri:** 1 hour topic study + 45 min DSA
- **Sat:** coding practice / hands-on project work for the week's topic
- **Sun:** revision + write answers to 10 interview questions in your own words (store in `/notes`)

**Rule:** for every topic, you should be able to (1) explain it in simple words, (2) write a small code example, (3) say where you used it or would use it.
