JAVA BACKEND INTERVIEW ROADMAP





1\. CORE JAVA



OOP:

\- Class

\- Object

\- Encapsulation

\- Inheritance

\- Polymorphism

\- Abstraction

\- Composition vs Inheritance



Java Basics:

\- Primitive vs Wrapper classes

\- Autoboxing / Unboxing

\- static

\- this

\- super

\- Constructor

\- Constructor chaining

\- Access modifiers -> public, private, protected, default

\- final

\- final vs finally vs finalize

\- Object class

\- Enum

\- Pass-by-value in Java



Methods:

\- Method overloading

\- Method overriding

\- Varargs



Interfaces \& Classes:

\- Interface

\- Abstract class

\- Interface vs Abstract class

\- Default methods

\- Static methods in interfaces



Object \& Memory Concepts:

\- == vs equals()

\- hashCode()

\- Immutable class

\- Shallow copy vs Deep copy

\- clone() basics



Nested Types:

\- Inner classes

\- Static nested classes

\- Anonymous classes



Generics:

\- Generic classes

\- Generic methods

\- <T>

\- <?>

\- <? extends T>

\- <? super T>



Control Constructs:

\- if-else

\- nested-if

\- for loop

\- enhanced for loop / foreach

\- while

\- do-while

\- switch-case

\- break

\- continue

\- labeled statements





2\. JVM \& MEMORY MANAGEMENT



\- JVM

\- JDK vs JRE vs JVM

\- Class Loader

\- Runtime Data Areas

\- Stack

\- Heap

\- Method Area / Metaspace

\- Garbage Collection

\- Strong references

\- Weak references

\- StackOverflowError

\- OutOfMemoryError





3\. EXCEPTION HANDLING



\- Exception hierarchy

\- Checked vs Unchecked exceptions

\- try

\- catch

\- finally

\- throw

\- throws

\- Custom exceptions

\- Multiple catch

\- Try-with-resources

\- Exception propagation

\- Best practices for exception handling





4\. COLLECTIONS



Collection Hierarchy:

\- Collection vs Collections

\- Iterable

\- List

\- Set

\- Queue

\- Map



List:

\- ArrayList

\- LinkedList

\- Vector



Set:

\- HashSet

\- LinkedHashSet

\- TreeSet



Map:

\- HashMap

\- LinkedHashMap

\- TreeMap

\- Hashtable

\- ConcurrentHashMap



Queue:

\- PriorityQueue

\- Deque

\- ArrayDeque



Important Concepts:

\- Hashing

\- hashCode() and equals()

\- HashMap internal working

\- HashSet internal working

\- Collision

\- Load factor

\- Initial capacity

\- Resize / Rehashing

\- Comparable

\- Comparator

\- Collections.sort()

\- Custom sorting





5\. JAVA 8+



\- Lambda expressions

\- Functional interfaces

\- Predicate

\- Function

\- Consumer

\- Supplier

\- Method references

\- Default methods

\- Static interface methods



Stream API:

\- stream()

\- map()

\- filter()

\- flatMap()

\- reduce()

\- sorted()

\- distinct()

\- limit()

\- skip()

\- count()

\- anyMatch()

\- allMatch()

\- noneMatch()

\- findFirst()

\- findAny()

\- Collectors

\- groupingBy()

\- partitioningBy()

\- joining()



\- Optional





6\. MULTITHREADING \& CONCURRENCY



Basics:

\- Process vs Thread

\- Thread lifecycle

\- Thread creation

\- Thread class

\- Runnable

\- Callable



Thread Control:

\- start()

\- run()

\- sleep()

\- join()

\- wait()

\- notify()

\- notifyAll()



Synchronization:

\- synchronized

\- volatile

\- Atomic classes

\- Lock

\- ReentrantLock



Concurrency:

\- ExecutorService

\- ThreadPool

\- Future

\- Concurrent collections



Problems:

\- Race condition

\- Deadlock

\- Starvation



Important Concepts:

\- Thread safety

\- Mutual exclusion

\- Executor vs Thread creation





7\. JDBC



\- JDBC architecture

\- Driver

\- Connection

\- Statement

\- PreparedStatement

\- CallableStatement

\- ResultSet

\- ResultSet types

\- Transactions

\- commit()

\- rollback()

\- Connection pooling

\- SQL injection

\- PreparedStatement vs Statement





8\. HTTP / REST APIs



HTTP:

\- HTTP request

\- HTTP response

\- Request headers

\- Response headers

\- Request body

\- Response body

\- Content-Type

\- Accept

\- Authorization

\- Cookies

\- Sessions



HTTP Methods:

\- GET

\- POST

\- PUT

\- PATCH

\- DELETE

\- OPTIONS

\- HEAD



HTTP Status Codes:

\- 2xx

\- 3xx

\- 4xx

\- 5xx

\- 200

\- 201

\- 204

\- 400

\- 401

\- 403

\- 404

\- 409

\- 422

\- 500

\- 502

\- 503



REST:

\- REST principles

\- Statelessness

\- Resource-based URLs

\- Idempotency

\- HTTP methods

\- API versioning

\- Pagination

\- Filtering

\- Sorting





9\. NETWORKING



\- Client vs Server

\- DNS

\- IP address

\- Port

\- TCP vs UDP

\- TCP 3-way handshake

\- HTTPS

\- TLS/SSL basics

\- Forward Proxy

\- Reverse Proxy

\- Load Balancer

\- CORS

\- Cookies

\- Sessions

\- JWT



Load Balancing:

\- Round Robin

\- Weighted Round Robin

\- Least Connections

\- IP Hash





10\. SERVLETS



\- Servlet

\- Servlet lifecycle

\- Servlet container

\- Request / Response

\- doGet()

\- doPost()

\- Session

\- Cookies

\- Filters

\- DispatcherServlet

\- Servlet vs Spring MVC





11\. HIBERNATE / JPA / SPRING DATA JPA



JPA:

\- Entity

\- Entity lifecycle

\- Persistence Context

\- First-level cache

\- Transactions

\- JPQL

\- Native queries



Relationships:

\- @OneToOne

\- @OneToMany

\- @ManyToOne

\- @ManyToMany

\- mappedBy

\- Owning side

\- Cascade

\- orphanRemoval



Fetching:

\- Lazy loading

\- Eager loading

\- N+1 problem

\- Entity Graph basics



Hibernate:

\- Hibernate architecture

\- Dirty checking

\- Session

\- SessionFactory

\- HQL



Spring Data JPA:

\- Repository

\- JpaRepository

\- CrudRepository

\- Derived query methods

\- @Query

\- Pagination

\- Sorting



Important:

\- JPA vs Hibernate

\- Hibernate vs Spring Data JPA

\- Persistence Context

\- Transactions

\- Optimistic locking / @Version





12\. SPRING CORE



\- IoC

\- Dependency Injection

\- Constructor Injection

\- Field Injection

\- Setter Injection

\- Bean

\- Bean lifecycle

\- Bean scopes

\- Component scanning

\- ApplicationContext



Annotations:

\- @Component

\- @Service

\- @Repository

\- @Controller

\- @Autowired

\- @Configuration

\- @Bean





13\. SPRING BOOT



\- Spring Boot

\- Spring Boot vs Spring Framework

\- Starter dependencies

\- Auto-configuration

\- application.properties

\- application.yml

\- Profiles

\- Configuration properties

\- Environment variables

\- Actuator

\- Logging



REST:

\- @RestController

\- @RequestMapping

\- @GetMapping

\- @PostMapping

\- @PutMapping

\- @PatchMapping

\- @DeleteMapping

\- @RequestParam

\- @PathVariable

\- @RequestBody

\- @ResponseBody

\- ResponseEntity



Application Architecture:

\- Controller

\- Service

\- Repository

\- DTO

\- Entity

\- Mapper



Validation:

\- @Valid

\- @NotNull

\- @NotBlank

\- @Size

\- @Email

\- Custom validation



Exception Handling:

\- @ExceptionHandler

\- @ControllerAdvice

\- @RestControllerAdvice

\- Global exception handling





14\. SPRING MVC



\- Spring MVC architecture

\- DispatcherServlet

\- Handler Mapping

\- Controller

\- Request processing

\- Message converters

\- Request parameters

\- Path variables

\- Request body

\- Response body

\- Exception handling





15\. SPRING SECURITY



Authentication:

\- Authentication

\- Authorization

\- AuthenticationManager

\- SecurityContext

\- SecurityContextHolder



Authorization:

\- Roles

\- Authorities

\- RBAC

\- Access control



Security:

\- SecurityFilterChain

\- Security filters

\- Password hashing

\- BCrypt

\- PasswordEncoder



JWT:

\- JWT structure

\- Access token

\- Refresh token

\- JWT authentication flow



Web Security:

\- CORS

\- CSRF

\- CORS vs CSRF





16\. SQL



SQL Basics:

\- SELECT

\- WHERE

\- DISTINCT

\- ORDER BY

\- GROUP BY

\- HAVING

\- LIMIT / OFFSET

\- CASE



Joins:

\- INNER JOIN

\- LEFT JOIN

\- RIGHT JOIN

\- FULL JOIN

\- CROSS JOIN

\- Self Join



Queries:

\- Subqueries

\- EXISTS

\- IN

\- UNION

\- UNION ALL

\- CTE



Database:

\- Primary Key

\- Foreign Key

\- Unique Key

\- Constraints

\- Composite Key

\- Normalization

\- Denormalization

\- Views



SQL Commands:

\- DDL

\- DML

\- DCL

\- TCL



Functions:

\- Aggregate functions

\- String functions

\- Date functions

\- Numeric functions

\- User-defined functions



Database Features:

\- Transactions

\- ACID

\- Isolation levels

\- Indexes

\- Composite indexes

\- Clustered vs non-clustered index basics

\- EXPLAIN / query execution plan

\- Query optimization

\- Triggers





17\. DSA



Big-O:

\- O(1)

\- O(log n)

\- O(n)

\- O(n log n)

\- O(n²)

\- Time complexity

\- Space complexity



Arrays:

\- Traversal

\- Searching

\- Linear Search

\- Binary Search

\- Two Pointers

\- Sliding Window



Sorting:

\- Bubble Sort

\- Selection Sort

\- Insertion Sort

\- Merge Sort

\- Quick Sort



Strings:

\- Character frequency

\- Anagrams

\- Palindrome

\- Duplicate characters



HashMap / HashSet:

\- Frequency counting

\- Duplicate detection

\- Two Sum



Stack:

\- Parentheses

\- Next Greater Element



Queue:

\- Basic Queue

\- Deque

\- Priority Queue



Linked List:

\- Singly Linked List

\- Doubly Linked List

\- Reverse Linked List

\- Detect Cycle

\- Find Middle

\- Merge Lists



Later:

\- Recursion

\- Trees

\- Binary Search Tree

\- Heap

\- Graph basics





18\. REDIS / CACHING



\- What is caching?

\- Why caching?

\- Redis

\- Key-value storage

\- TTL

\- Cache hit / miss

\- Cache-aside pattern

\- Cache invalidation

\- Eviction policies

\- Redis data types

\- Redis vs Database





19\. KAFKA / MESSAGE QUEUES



Message Queues:

\- Producer

\- Consumer

\- Message

\- Queue

\- Topic



Kafka:

\- Broker

\- Topic

\- Partition

\- Producer

\- Consumer

\- Consumer Group

\- Offset

\- Replication

\- Ordering

\- Retention



RabbitMQ:

\- Producer

\- Consumer

\- Queue

\- Exchange

\- Routing Key



Kafka vs RabbitMQ





20\. SYSTEM DESIGN



Fundamentals:

\- Client → Server architecture

\- REST API architecture

\- Reverse Proxy

\- Forward Proxy

\- Load Balancer

\- Horizontal Scaling

\- Vertical Scaling

\- Caching

\- Database scaling

\- Replication

\- Sharding

\- SQL vs NoSQL

\- CAP theorem

\- Consistency

\- Availability

\- Message Queues

\- Microservices

\- API Gateway

\- Rate Limiting

\- Authentication

\- Authorization

\- Logging

\- Monitoring

\- Retry

\- Timeout

\- Circuit Breaker

\- Idempotency



Load Balancing:

\- Round Robin

\- Weighted Round Robin

\- Least Connections

\- IP Hash



Practice Designs:

\- URL Shortener

\- E-commerce Order System

\- Notification System



Example Architecture:



Client

&#x20;  ↓

Load Balancer

&#x20;  ↓

API Gateway

&#x20;  ↓

Spring Boot Services

&#x20;  ↓

Redis

&#x20;  ↓

Database



Spring Boot Services

&#x20;  ↓

Kafka

&#x20;  ↓

Other Services





21\. JAVASCRIPT



\- var

\- let

\- const

\- Primitive / Reference types

\- Scope

\- Hoisting

\- Functions

\- Arrow functions

\- Closures

\- this

\- Array methods

\- map()

\- filter()

\- reduce()

\- Promises

\- async / await

\- Event Loop

\- Fetch API

\- DOM basics





22\. REACT.JS



\- Components

\- Props

\- State

\- Conditional rendering

\- Event handling

\- Forms

\- API integration



Hooks:

\- useState

\- useEffect

\- useContext

\- useCallback

\- useMemo

\- useRef



\- Component lifecycle basics

\- Controlled components





23\. TYPESCRIPT



\- Types

\- Interfaces

\- Type aliases

\- Union types

\- Optional properties

\- Generics

\- Enums

\- Type narrowing

\- Basic utility types





24\. AI / LLM



AI Basics:

\- AI vs ML vs Deep Learning

\- LLM

\- Tokens

\- Context window

\- Prompting

\- Temperature

\- Embeddings



LLM Applications:

\- OpenAI API integration

\- Chatbot

\- Conversation history

\- Function / Tool calling

\- RAG

\- Vector database

\- Semantic search

\- AI Agents

\- MCP



Java Integration:

\- Integrating LLM APIs with Spring Boot

\- Calling AI APIs

\- Handling responses

\- Error handling

\- Authentication/API keys

