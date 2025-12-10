# COBOL to PL/I Conversion Help

Tartalom

[COBOL to PL/I Conversion Help 1](#_Toc216026900)

[Chapter 1 — Introduction 5](#_Toc216026901)

[1.1 Purpose of This Manual 5](#_Toc216026902)

[1.2 What Is PL/I? 6](#_Toc216026903)

[1.3 Why COBOL Programmers Encounter PL/I 6](#_Toc216026904)

[1.4 Fundamental Philosophical Differences Between COBOL and PL/I 7](#_Toc216026905)

[Chapter 2 — Language Philosophy and Architecture 8](#_Toc216026906)

[2.1 COBOL’s Architecture 8](#_Toc216026907)

[2.2 PL/I’s Architecture 9](#_Toc216026908)

[2.3 Structural Comparison 9](#_Toc216026909)

[2.4 Example Comparison 10](#_Toc216026910)

[Chapter 3 — Data Declaration and Typing 10](#_Toc216026911)

[3.1 COBOL Data Types (PIC Clauses) 10](#_Toc216026912)

[3.2 PL/I Data Types 11](#_Toc216026913)

[3.3 Example: COBOL vs PL/I structure 12](#_Toc216026914)

[3.4 Arrays 12](#_Toc216026915)

[3.5 Dynamic Structures 12](#_Toc216026916)

[Chapter 4 — Storage Classes and Lifetimes 13](#_Toc216026917)

[4.1 COBOL Storage 13](#_Toc216026918)

[4.2 PL/I Storage Classes 13](#_Toc216026919)

[4.3 CONTROLLED vs BASED 13](#_Toc216026920)

[Chapter 5 — Control Flow 15](#_Toc216026921)

[5.1 DO Loops vs PERFORM 15](#_Toc216026922)

[5.2 IF Statements 15](#_Toc216026923)

[5.3 SELECT WHEN (COBOL EVALUATE) 15](#_Toc216026924)

[5.4 Exception Handling (ON-units) 16](#_Toc216026925)

[Chapter 6 — Structures (Records) in PL/I vs COBOL 17](#_Toc216026926)

[6.1 COBOL Records: Rigid, Hierarchical 17](#_Toc216026927)

[6.2 PL/I Structures: Flexible and Typed 18](#_Toc216026928)

[6.3 Arrays of Structures (PL/I-only) 18](#_Toc216026929)

[6.4 Nested Structures and True Typing 19](#_Toc216026930)

[6.5 Structure Assignments 19](#_Toc216026931)

[6.6 Unions (REDEFINES Equivalent) 19](#_Toc216026932)

[Chapter 7 — Strings and Character Handling 20](#_Toc216026933)

[7.1 COBOL Strings 20](#_Toc216026934)

[7.2 PL/I Character Types 20](#_Toc216026935)

[7.3 Powerful String Built-ins 21](#_Toc216026936)

[7.4 Reference Modification in PL/I 21](#_Toc216026937)

[7.5 Concatenation 22](#_Toc216026938)

[Chapter 8 — Arrays and Multidimensional Data 23](#_Toc216026939)

[8.1 COBOL Arrays 23](#_Toc216026940)

[8.2 PL/I Arrays 23](#_Toc216026941)

[8.3 Array Slicing and Whole-Array Operations 23](#_Toc216026942)

[8.4 Dynamic Arrays 25](#_Toc216026943)

[Chapter 9 — Pointers, BASED, CONTROLLED, and Dynamic Memory 26](#_Toc216026944)

[9.1 POINTER Type 26](#_Toc216026945)

[9.2 BASED Variables 26](#_Toc216026946)

[9.3 CONTROLLED Variables 26](#_Toc216026947)

[9.4 Linked Lists Example 27](#_Toc216026948)

[Chapter 10 — Areas and Storage Pools 28](#_Toc216026949)

[Chapter 11 — File Handling: PL/I vs COBOL 29](#_Toc216026950)

[11.1 COBOL File Model (FD / SELECT) 29](#_Toc216026951)

[11.2 PL/I File Model (FILE Declarations) 30](#_Toc216026952)

[11.3 Sequential Read Logic 30](#_Toc216026953)

[11.4 Writing Records 31](#_Toc216026954)

[11.5 Keyed / Indexed Files 31](#_Toc216026955)

[Chapter 12 — Exception Handling (Conditions and ON-units) 33](#_Toc216026956)

[12.1 Conditions 33](#_Toc216026957)

[12.2 ON-units: Local Exception Handlers 33](#_Toc216026958)

[12.3 Comparison with COBOL 34](#_Toc216026959)

[12.4 Explicit SIGNAL 34](#_Toc216026960)

[12.5 CLEANUP Equivalent 34](#_Toc216026961)

[Chapter 13 — Procedures and Modularity 35](#_Toc216026962)

[13.1 COBOL CALL vs PL/I PROC 35](#_Toc216026963)

[13.2 PL/I Procedure Declaration 35](#_Toc216026964)

[13.3 Parameter Passing 35](#_Toc216026965)

[13.4 Nested Procedures 36](#_Toc216026966)

[13.5 Recursion 36](#_Toc216026967)

[Chapter 14 — SQL in PL/I vs COBOL 37](#_Toc216026968)

[14.1 Host Variables 37](#_Toc216026969)

[14.2 SQLCA 37](#_Toc216026970)

[14.3 Cursors 37](#_Toc216026971)

[Chapter 15 — Built-in Function Reference (EXTENDED) 39](#_Toc216026972)

[15.1 String Functions 39](#_Toc216026973)

[15.2 Numeric Functions 39](#_Toc216026974)

[15.3 Bit Functions 40](#_Toc216026975)

[15.4 Array Functions 40](#_Toc216026976)

[15.5 Condition Functions 40](#_Toc216026977)

[15.6 Miscellaneous Functions 41](#_Toc216026978)

[Chapter 16 — Advanced Data Features (OVERLAY, UNION, AREA) 42](#_Toc216026979)

[16.1 UNION (Advanced REDEFINES) 42](#_Toc216026980)

[16.2 OVERLAY 42](#_Toc216026981)

[16.3 AREA 43](#_Toc216026982)

[16.4 STORAGE Class 43](#_Toc216026983)

[Chapter 17 — Concurrency and Tasking 44](#_Toc216026984)

[17.1 TASK Statements 44](#_Toc216026985)

[17.2 Event Handling 44](#_Toc216026986)

[Chapter 18 — Debugging Techniques and ON Conditions 46](#_Toc216026987)

[18.1 ON ERROR for Debugging 46](#_Toc216026988)

[18.2 ON UNDEFINEDFILE, ON FINISH 46](#_Toc216026989)

[18.3 Built-in Debugging Functions 46](#_Toc216026990)

[18.4 Compiler Options for Debugging 47](#_Toc216026991)

[Chapter 19 — Performance Guidelines 48](#_Toc216026992)

[19.1 Use FIXED BINARY Whenever Possible 48](#_Toc216026993)

[19.2 Avoid Excessive POINTER and BASED Use 48](#_Toc216026994)

[19.3 Use VARYING Strings for Performance 48](#_Toc216026995)

[19.4 Avoid Unnecessary ON-units 48](#_Toc216026996)

[19.5 Inline Arithmetic (Expression-Oriented) 48](#_Toc216026997)

[19.6 Compiler Optimization 49](#_Toc216026998)

[Chapter 20 — Migration Strategies from COBOL to PL/I 50](#_Toc216026999)

[20.1 Translate Control Flow First 50](#_Toc216027000)

[20.2 Translate Data Structures 50](#_Toc216027001)

[20.3 Replace COPY Libraries with %INCLUDE 50](#_Toc216027002)

[20.4 Convert File Logic 50](#_Toc216027003)

[20.5 Convert String Handling 51](#_Toc216027004)

[20.6 Handling COMP-3 Fields 51](#_Toc216027005)

[20.7 Testing and Validation 51](#_Toc216027006)

[Chapter 21 — Idiomatic PL/I for COBOL Programmers 52](#_Toc216027007)

[21.1 Whole-Array Operations 52](#_Toc216027008)

[21.2 Whole-Structure Assignment 52](#_Toc216027009)

[21.3 Selective Exception Handling 52](#_Toc216027010)

[21.4 Dynamic Buffers 52](#_Toc216027011)

[Chapter 22 — Common Pitfalls for COBOL Programmers 53](#_Toc216027012)

[22.1 Uninitialized AUTOMATIC Variables 53](#_Toc216027013)

[22.2 Precision Errors 53](#_Toc216027014)

[22.3 Pointer Misuse 53](#_Toc216027015)

[22.4 Overreliance on ON-units 53](#_Toc216027016)

[22.5 VARYING String Length 53](#_Toc216027017)

[Chapter 23 — Comprehensive COBOL → PL/I Feature Equivalence Matrix 55](#_Toc216027018)

[23.1 Program Structure 55](#_Toc216027019)

[23.2 Data Types 55](#_Toc216027020)

[23.3 Control Flow 56](#_Toc216027021)

[23.4 File I/O 56](#_Toc216027022)

[23.5 Strings 57](#_Toc216027023)

[23.6 Arithmetic 57](#_Toc216027024)

[23.7 SQL 58](#_Toc216027025)

[23.8 Error Handling 58](#_Toc216027026)

[23.9 Modularity 58](#_Toc216027027)

[23.10 Memory Model 58](#_Toc216027028)

[Chapter 24 — Migration Checklist (Production-Ready) 60](#_Toc216027029)

[24.1 Data Structure Migration Checklist 60](#_Toc216027030)

[24.2 Control Flow Checklist 60](#_Toc216027031)

[24.3 String Handling Checklist 60](#_Toc216027032)

[24.4 File Handling Checklist 60](#_Toc216027033)

[24.5 SQL Migration Checklist 61](#_Toc216027034)

[24.6 Exception Handling Checklist 61](#_Toc216027035)

[24.7 Best Practice Checklist 61](#_Toc216027036)

[Chapter 25 — Professional Glossary (COBOL → PL/I) 62](#_Toc216027037)

[25.1 A–C 62](#_Toc216027038)

[25.2 D–H 62](#_Toc216027039)

[25.3 I–Q 62](#_Toc216027040)

[25.4 R–Z 62](#_Toc216027041)

[Chapter 26 — Full Alphabetical Index 64](#_Toc216027042)

[Chapter 27 — Final Professional Recommendations 67](#_Toc216027043)

[Literature links: IBM Enterprise PL/I for z/OS - IBM Documentation 67](#_Toc216027044)

## Chapter 1 — Introduction

### 1.1 Purpose of This Manual

This manual is designed for **experienced COBOL programmers** who must learn or maintain PL/I applications.
It assumes:

* knowledge of mainframe concepts (z/OS, JCL, datasets)
* experience with structured COBOL
* familiarity with record-based business processing

Its purpose is to explain:

* **what PL/I is**,
* **how it differs from COBOL**,
* **how to write PL/I effectively**,
* **how to translate business logic**,
* **how to understand PL/I systems you inherit**,
* **how to use PL/I’s powerful features safely**.

Most importantly, this manual is **feature-by-feature comparative**, not a generic language tutorial.
Every major concept is shown with a **COBOL equivalent**, with PL/I’s extended capabilities explained clearly.

### 1.2 What Is PL/I?

PL/I (“Programming Language One”) is an IBM-developed language intended to unify:

* COBOL’s business data handling,
* FORTRAN’s numeric and scientific abilities,
* ALGOL’s structured control constructs,
* Assembler’s low-level control.

It was created to be:

* stronger than COBOL in computation,
* stronger than FORTRAN in data handling,
* stronger than ALGOL in I/O and exceptions,
* and strong enough for systems programming.

### 1.3 Why COBOL Programmers Encounter PL/I

Mainframe shops typically encounter PL/I because:

* Large IBM organizations use a **mix of PL/I and COBOL**.
* PL/I is heavily used in:
  + financial calculations
  + algorithms requiring precision and speed
  + IMS/Db2 batch systems
  + telecommunication software
  + OS/390 and z/OS system utilities
* Many existing systems were written in PL/I in the 1970s–1990s and are still operational.

COBOL programmers inheriting PL/I code must be able to:

* Read and understand PL/I logic
* Trace logic across nested procedures
* Understand PL/I file handling
* Translate PL/I numerical or structural constructs
* Modify logic safely

### 1.4 Fundamental Philosophical Differences Between COBOL and PL/I

COBOL is:

* **business-oriented**
* **record-focused**
* **verb-oriented (“MOVE”, “PERFORM”, “DISPLAY”)**
* **division-structured**
* **simple but rigid**

PL/I is:

* **general-purpose**
* **expression-oriented**
* **block-structured**
* **free-form**
* **feature-rich**
* supports recursion, concurrency, dynamic memory, pointers, exceptions

These differences affect:

* program layout
* data declarations
* memory handling
* control flow
* error handling
* file I/O
* SQL integration
* and ultimately the mental model used for programming

This chapter explains these differences to prepare you for the deeper sections ahead.

## Chapter 2 — Language Philosophy and Architecture

### 2.1 COBOL’s Architecture

COBOL programs are organized into **divisions**:

1. IDENTIFICATION DIVISION
2. ENVIRONMENT DIVISION
3. DATA DIVISION
4. PROCEDURE DIVISION

This structure enforces a **rigid layered model**:

* All data must be declared in DATA DIVISION.
* All executable logic must be in PROCEDURE DIVISION.
* No intermixing of declarations and statements.
* Formatting rules (columns, paragraph names) historically mattered.

**Execution Model:**
COBOL executes **top-to-bottom**, invoking paragraphs through PERFORM.

**Data Model:**
Data is defined as hierarchical **records** using PIC clauses.

### 2.2 PL/I’s Architecture

PL/I eliminates divisions entirely.

A PL/I program consists of:

* **procedures** (PROC ... END)
* **blocks** (DO ... END)
* **declarations** (DCL)
* **statements**
* **exception handlers** (ON ... units)
* optional submodules (%INCLUDE)

PL/I is **free-form**, like C, Java, or Python:

* No required divisions
* No required structure
* Declarations may appear anywhere in a block
* Procedures may be nested
* Recursion allowed
* Exception handling part of the language

### 2.3 Structural Comparison

| **Feature**          | **COBOL**            | **PL/I**                |
| -------------------- | -------------------- | ----------------------- |
| Program organization | Fixed divisions      | Free-form, procedural   |
| Execution            | Paragraphs + PERFORM | Procedures + CALL       |
| Nesting              | No                   | Yes (nested procedures) |
| Declarations         | Data Division only   | Anywhere in block       |
| Exceptions           | Declaratives         | ON-units                |
| Recursion            | Not allowed          | Allowed                 |
| Dynamic memory       | Not available        | Full support            |
| Arrays               | Only 1D              | Multi-dimensional       |

### 2.4 Example Comparison

**COBOL:**

IDENTIFICATION DIVISION.

PROGRAM-ID. SAMPLE.

PROCEDURE DIVISION.

PERFORM A-PARA.

STOP RUN.

A-PARA.

DISPLAY "HELLO".

EXIT.

**PL/I:**

SAMPLE: PROC OPTIONS(MAIN);

CALL A\_PARA;

END SAMPLE;

A\_PARA: PROC;

PUT SKIP LIST('HELLO');

END A\_PARA;

## Chapter 3 — Data Declaration and Typing

This chapter is critical: PL/I’s type system is **richer, stricter, and far more powerful** than COBOL’s.

### 3.1 COBOL Data Types (PIC Clauses)

COBOL uses:

* PIC X(n) → character
* PIC 9(n) → numeric
* COMP, COMP-3 → packed/binary
* OCCURS → arrays
* REDEFINES → unions / overlays
* VALUE → initial value

Examples:

01 EMPLOYEE.

05 ID PIC 9(5).

05 NAME PIC X(20).

05 SALARY PIC 9(7)V99 COMP-3.

### 3.2 PL/I Data Types

PL/I has explicit types, each with purpose and precision.

**Numeric Types:**

* FIXED BINARY(n)
* FIXED DECIMAL(p,s)
* FLOAT
* COMPLEX

**Character Types:**

* CHAR(n)
* CHAR(n) VARYING
* GRAPHIC(n)

**Bit Types:**

* BIT(n)

**Structures:**

* Explicit hierarchical structures (STRUCT)

**Pointer Types:**

* POINTER
* OFFSET
* AREA

### 3.3 Example: COBOL vs PL/I structure

**COBOL:**

01 PERSON.

05 NAME PIC X(20).

05 AGE PIC 9(3).

**PL/I:**

DCL 1 PERSON,

2 NAME CHAR(20),

2 AGE FIXED DEC(3,0);

### 3.4 Arrays

COBOL:

05 SALES OCCURS 12 TIMES PIC 9(5).

PL/I:

DCL SALES(12) FIXED DEC(5,0);

PL/I supports **multi-dimensional arrays**:

DCL MATRIX(12, 31) FIXED BIN;

COBOL does not (or not so simply).

### 3.5 Dynamic Structures

COBOL does not support dynamic memory.

PL/I:

DCL NODE POINTER;

DCL 1 NODE\_STRUCT BASED(NODE),

2 VAL FIXED BIN,

2 NEXT POINTER;

ALLOCATE NODE\_STRUCT;

This allows linked lists, trees, queues in PL/I.

## Chapter 4 — Storage Classes and Lifetimes

### 4.1 COBOL Storage

| **COBOL Section** | **Lifetime**         |
| ----------------- | -------------------- |
| WORKING-STORAGE   | Entire run           |
| LOCAL-STORAGE     | Per invocation       |
| LINKAGE           | Controlled by caller |
| FILE SECTION      | Static               |

No dynamic allocation exists.

### 4.2 PL/I Storage Classes

| **PL/I Class** | **Description**             | **Equivalent**                              |
| -------------- | --------------------------- | ------------------------------------------- |
| STATIC         | Exists entire run           | WORKING-STORAGE                             |
| AUTOMATIC      | Per block activation        | LOCAL-STORAGE                               |
| CONTROLLED     | Allocated via ALLOCATE      | None in COBOL                               |
| BASED          | Exists only through pointer | REDEFINES + POINTER (not possible in COBOL) |

### 4.3 CONTROLLED vs BASED

Example:

DCL P POINTER;

DCL RECORD CONTROLLED CHAR(100);

ALLOCATE RECORD; /\* storage appears \*/

FREE RECORD; /\* storage disappears \*/

BASED example:

DCL P POINTER;

DCL 1 NODE BASED(P),

2 VALUE FIXED BIN,

2 NEXT POINTER;

ALLOCATE NODE;

P->VALUE = 100;

## Chapter 5 — Control Flow

### 5.1 DO Loops vs PERFORM

**COBOL**:

PERFORM VARYING I FROM 1 BY 1 UNTIL I > 10

DISPLAY I

END-PERFORM.

**PL/I:**

DO I = 1 TO 10;

PUT SKIP LIST(I);

END;

PL/I supports:

* DO WHILE
* DO UNTIL
* infinite DO loops
* LEAVE and ITERATE (COBOL lacks ITERATE)

### 5.2 IF Statements

COBOL:

IF A > B THEN DISPLAY "A".

PL/I:

IF A > B THEN PUT SKIP LIST('A');

### 5.3 SELECT WHEN (COBOL EVALUATE)

**COBOL**:

EVALUATE X

WHEN 1 DISPLAY "ONE"

WHEN 2 DISPLAY "TWO"

WHEN OTHER DISPLAY "OTHER"

END-EVALUATE.

**PL/I:**

SELECT;

WHEN (X = 1) PUT LIST('ONE');

WHEN (X = 2) PUT LIST('TWO');

OTHERWISE PUT LIST('OTHER');

END;

### 5.4 Exception Handling (ON-units)

**PL/I:**

ON ZERODIVIDE PUT SKIP LIST('Division by zero');

COBOL does not have an equivalent general exception model.

### Chapter 6 — Structures (Records) in PL/I vs COBOL

Structures (records) are one of the most important concepts for COBOL programmers, because PL/I’s structure system is **far more powerful** than COBOL’s hierarchical records.

### 6.1 COBOL Records: Rigid, Hierarchical

A COBOL record is:

* strictly hierarchical
* composed of levels (01, 05, 10, etc.)
* fixed at compile time
* cannot be resized dynamically
* always has a fixed memory location
* can use REDEFINES to simulate unions

Example COBOL record:

01 EMPLOYEE-REC.

05 EMP-ID PIC 9(5).

05 EMP-NAME PIC X(20).

05 EMP-SALARY PIC 9(7)V99.

Characteristics:

* size is fixed
* structure cannot change at runtime
* field types limited to PIC specifications
* REDEFINES overlaps memory
* OCCURS creates arrays
* No pointers

### 6.2 PL/I Structures: Flexible and Typed

PL/I structures are declared with DCL and level numbers:

DCL 1 EMPLOYEE,

2 ID FIXED DEC(5,0),

2 NAME CHAR(20),

2 SALARY DECIMAL(9,2);

Differences from COBOL:

| **Feature**              | **COBOL**           | **PL/I**                    |
| ------------------------ | ------------------- | --------------------------- |
| Type control             | PIC, not true types | Strong numeric/string types |
| Unions                   | REDEFINES           | UNION attribute             |
| Pointers                 | No                  | Yes                         |
| Dynamic records          | Impossible          | CONTROLLED, BASED, ALLOCATE |
| Arrays inside structures | Yes                 | Yes                         |
| Arrays of structures     | Limited             | Fully supported             |
| Multidimensional         | No                  | Yes                         |

### 6.3 Arrays of Structures (PL/I-only)

DCL 1 EMPLOYEES(100),

2 ID FIXED BINARY(31),

2 NAME CHAR(20),

2 SALARY DECIMAL(7,2);

COBOL would require:

* OCCURS on each field
* no syntactical grouping
* manual indexing

### 6.4 Nested Structures and True Typing

PL/I supports deeper nesting:

DCL 1 DEPT,

2 DEPTNO FIXED BIN,

2 MANAGER,

3 NAME CHAR(20),

3 PHONE CHAR(15),

2 EMPLOYEE(50),

3 ID FIXED BIN,

3 SALARY DECIMAL(9,2);

This is **functionally impossible** to express cleanly in COBOL.

### 6.5 Structure Assignments

PL/I supports whole-structure assignment:

EMP2 = EMP1;

COBOL requires field-by-field MOVE.

### 6.6 Unions (REDEFINES Equivalent)

**COBOL:**

05 A PIC 9(4).

05 B REDEFINES A PIC X(4).

**PL/I:**

DCL 1 U UNION,

2 A FIXED BIN,

2 B CHAR(4);

PL/I unions are safer and better-defined.

## Chapter 7 — Strings and Character Handling

COBOL’s string system is **primitive**. PL/I’s is extremely advanced.

## 7.1 COBOL Strings

COBOL strings are:

* fixed-length
* space-filled
* manipulated with:
  + STRING
  + UNSTRING
  + INSPECT
  + MOVE CORRESPONDING
* stored in PIC X(n)

Common issues:

* trailing spaces
* no built-in substring function
* no trimming without INSPECT
* complicated concatenation

### 7.2 PL/I Character Types

PL/I supports:

**Fixed strings:**

DCL NAME CHAR(20);

**Varying strings:**

DCL LINE CHAR(100) VARYING;

VARYING strings:

* track their own length
* do not pad with spaces
* behave like modern languages (Java/Python)

### 7.3 Powerful String Built-ins

PL/I provides dozens of functions:

| **Function** | **Purpose**                    |
| ------------ | ------------------------------ |
| SUBSTR       | Extract substring              |
| INDEX        | Find substring                 |
| VERIFY       | Scan for unacceptable chars    |
| TRANSLATE    | Map characters                 |
| REPEAT       | Repeat character/string        |
| LENGTH       | Length of string               |
| TRIM         | Remove leading/trailing spaces |

Example:

DCL LASTNAME CHAR(20);

LASTNAME = SUBSTR(FULLNAME, 6, 15);

COBOL would require:

* INSPECT
* MOVE with reference modification
* manual logic

### 7.4 Reference Modification in PL/I

COBOL:

MOVE FULLNAME(6:15) TO LASTNAME.

PL/I equivalent using SUBSTR:

LASTNAME = SUBSTR(FULLNAME, 6, 15);

### 7.5 Concatenation

**COBOL:**

STRING A B C INTO RESULT

**PL/I:**

RESULT = A || B || C;

Simple, clear, powerful.

## Chapter 8 — Arrays and Multidimensional Data

### 8.1 COBOL Arrays

COBOL uses OCCURS:

05 SALES OCCURS 12 TIMES PIC 9(5).

Limitations:

* Only 1D arrays allowed
* OCCURS DEPENDING ON does not allocate dynamically
* No true multidimensional syntax

### 8.2 PL/I Arrays

PL/I supports:

**1D:**

DCL SALES(12) FIXED DEC(5,0);

**2D:**

DCL MATRIX(10, 20) FLOAT;

**3D and beyond:**

DCL GRID(10, 10, 10) FIXED BIN;

**Arrays of structures:**

DCL EMP(100) LIKE EMPLOYEE;

### 8.3 Array Slicing and Whole-Array Operations

PL/I supports operations like:

TOTAL = SUM(SALES);

MAXVAL = MAX(SALES);

COBOL requires:

* writing loops
* manual accumulation
* no built-in aggregations

## 8.4 Dynamic Arrays

Using BASED:

DCL P POINTER;

DCL ARR(\*) BASED(P) FIXED BIN;

ALLOCATE ARR(100);

COBOL cannot do this.

## Chapter 9 — Pointers, BASED, CONTROLLED, and Dynamic Memory

PL/I is unique among mainframe high-level languages (other than C) in offering a full pointer/memory model.

This section is extremely important because PL/I systems often use complex pointer-based data structures.

### 9.1 POINTER Type

PL/I pointer equivalent of C pointers:

DCL P POINTER;

Holds memory addresses.

### 9.2 BASED Variables

BASED variables do not exist in memory until a pointer points to them.

DCL NODE POINTER;

DCL 1 NODE\_STRUCT BASED(NODE),

2 VAL FIXED BIN,

2 NEXT POINTER;

Equivalent to C structs.

COBOL has no equivalent.

### 9.3 CONTROLLED Variables

Dynamic allocation like malloc:

DCL RECORD CONTROLLED CHAR(80);

ALLOCATE RECORD;

FREE RECORD;

Allows:

* dynamic buffers
* variable-sized structures
* dynamic arrays

COBOL cannot do dynamic memory.

### 9.4 Linked Lists Example

DCL HEAD POINTER;

DCL 1 NODE BASED(HEAD),

2 VALUE FIXED BIN,

2 NEXT POINTER;

ALLOCATE NODE;

HEAD->VALUE = 10;

HEAD->NEXT = NULL;

COBOL cannot create linked lists without vendor hacks.

## Chapter 10 — Areas and Storage Pools

PL/I offers **AREAS**, which are user-defined memory pools:

DCL WORKAREA AREA(1024);

Objects can be allocated inside areas:

ALLOCATE X IN(WORKAREA);

Advantages:

* memory locality
* garbage-collection style frees
* isolated regions for temporary buffers

Advanced topic, powerful in systems programming.

## Chapter 11 — File Handling: PL/I vs COBOL

File handling is one of the most important areas for COBOL developers transitioning to PL/I.
While COBOL’s file system is built around the **FILE SECTION**, PL/I uses **FILE variables** combined with READ/WRITE/GET/PUT operations.

This chapter explains:

* Sequential files
* Keyed/indexed files
* Record formats
* End-of-file handling
* Error handling
* Mapping COBOL FD/SELECT → PL/I FILE

### 11.1 COBOL File Model (FD / SELECT)

COBOL describes files in:

* ENVIRONMENT DIVISION (SELECT, ASSIGN)
* FILE SECTION (FD, record layouts)

Example:

SELECT INFILE ASSIGN TO "DATA.IN".

FD INFILE.

01 IN-REC.

05 ID PIC 9(5).

05 NAME PIC X(20).

Operations:

READ INFILE INTO IN-REC AT END MOVE 1 TO EOF-FLAG.

WRITE OUT-REC.

REWRITE OUT-REC.

DELETE RECORD.

COBOL file I/O is **verb-oriented** and tightly bound to the FD structure.

### 11.2 PL/I File Model (FILE Declarations)

PL/I declares files using DCL:

DCL INFILE FILE RECORD INPUT;

DCL OUTFILE FILE RECORD OUTPUT;

* No FD
* No SELECT statements
* No division restrictions
* Record layout defined separately as structures or buffers

Example record:

DCL 1 INREC,

2 ID FIXED BIN(31),

2 NAME CHAR(20);

Reading:

READ FILE(INFILE) INTO(INREC);

Writing:

WRITE FILE(OUTFILE) FROM(INREC);

### 11.3 Sequential Read Logic

PL/I sequential loop:

OPEN FILE(INFILE);

ON ENDFILE(INFILE) EOF\_FLAG = 'Y';

DO WHILE(EOF\_FLAG ^= 'Y');

READ FILE(INFILE) INTO(INREC);

/\* Handle INREC \*/

END;

CLOSE FILE(INFILE);

Comparison:

| **Feature**    | **COBOL** | **PL/I**                 |
| -------------- | --------- | ------------------------ |
| EOF handling   | AT END    | ON ENDFILE               |
| File layout    | FD        | Structure or CHAR buffer |
| Read statement | READ      | READ FILE(...)           |
| Writes         | WRITE     | WRITE FILE(...)          |

### 11.4 Writing Records

OUTREC.ID = 12345;

OUTREC.NAME = 'JOHN SMITH';

WRITE FILE(OUTFILE) FROM(OUTREC);

PL/I fully supports formatted output via:

* LIST format (PUT LIST(...))
* EDIT format (PUT EDIT(...))

### 11.5 Keyed / Indexed Files

PL/I supports indexed (VSAM-like) files:

DCL CUST FILE KEYED INPUT;

DCL KEYVAL CHAR(10);

DCL REC CHAR(80);

READ FILE(CUST) SET(KEYVAL) INTO(REC);

Operations:

* READ … SET(KEY)
* READ … KEY(keyvalue)
* WRITE … KEY(keyvalue)
* REWRITE
* DELETE

COBOL equivalent is:

READ CUSTFILE INTO REC KEY IS CUSTKEY

INVALID KEY

...

END-READ.

PL/I uses **ON ERROR** to handle bad keys.

## Chapter 12 — Exception Handling (Conditions and ON-units)

PL/I’s **condition handling** is one of the most powerful parts of the language.
It is the equivalent of:

* COBOL AT END
* COBOL INVALID KEY
* C EXCEPTIONS
* Java TRY/CATCH

all combined.

### 12.1 Conditions

A PL/I **condition** is an event such as:

* ZERODIVIDE
* OVERFLOW
* UNDERFLOW
* ENDFILE
* ERROR
* CONVERSION
* FIXEDOVERFLOW
* SUBSCRIPTRANGE
* SIZE
* VALUE
* USER-DEFINED CONDITIONS

### 12.2 ON-units: Local Exception Handlers

Example:

ON ZERODIVIDE PUT SKIP LIST('Division by zero');

X = A / B;

If B = 0, the ON-unit runs.

### 12.3 Comparison with COBOL

| **COBOL**                   | **PL/I**                 |
| --------------------------- | ------------------------ |
| AT END                      | ON ENDFILE               |
| INVALID KEY                 | ON ERROR                 |
| Declaratives                | ON-units                 |
| No division by zero handler | ON ZERODIVIDE            |
| No structured exceptions    | Full condition framework |

PL/I conditions can be:

* turned on/off
* used lexically
* nested
* signaled explicitly (SIGNAL condition\_name)

### 12.4 Explicit SIGNAL

IF AMOUNT < 0 THEN SIGNAL NEGATIVE\_VALUE;

This is a custom exception, catchable by:

ON NEGATIVE\_VALUE PUT SKIP LIST('Error: Negative amount');

### 12.5 CLEANUP Equivalent

PL/I supports ON UNDEFINEDFILE, ON ERROR, ON FINISH for transaction safety.

COBOL has no general equivalent.

## Chapter 13 — Procedures and Modularity

PL/I procedures are far more advanced than COBOL paragraphs.

### 13.1 COBOL CALL vs PL/I PROC

**COBOL:**

CALL 'ROUTINE' USING A B C.

**PL/I:**

CALL ROUTINE(A, B, C);

### 13.2 PL/I Procedure Declaration

MYPROC: PROC(A, B) RETURNS(FIXED BIN);

DCL A FIXED BIN;

DCL B FIXED BIN;

RETURN (A + B);

END MYPROC;

### 13.3 Parameter Passing

| **Mode** | **Meaning**              |
| -------- | ------------------------ |
| Default  | By reference             |
| VALUE    | Passed by value          |
| OPTIONAL | Parameter may be omitted |

Example:

PROC(X, Y, Z) OPTIONS(MAIN);

DCL X FIXED BIN VALUE;

COBOL:

* Always BY REFERENCE
* No optional parameters
* No return values from CALL

PL/I allows **return values** and **expression-oriented calls**.

### 13.4 Nested Procedures

PL/I:

MAIN: PROC OPTIONS(MAIN);

INNER: PROC; ... END INNER;

END MAIN;

COBOL cannot nest procedures.

### 13.5 Recursion

PL/I supports:

FACT: PROC(N) RETURNS(FIXED BIN);

IF N = 0 THEN RETURN(1);

RETURN N \* FACT(N - 1);

END;

COBOL does not allow recursive calls (except nonstandard extensions).

## Chapter 14 — SQL in PL/I vs COBOL

Both languages use **EXEC SQL**, but with differences.

### 14.1 Host Variables

**COBOL:**

EXEC SQL

SELECT NAME INTO :WS-NAME

FROM EMP

WHERE ID = :WS-ID

END-EXEC.

**PL/I:**

EXEC SQL

SELECT NAME INTO :NAME

FROM EMP

WHERE ID = :ID;

PL/I variables must be declared with DCL instead of PIC.

### 14.2 SQLCA

In PL/I:

DCL SQLCA LIKE SQLCA\_DEF;

COBOL uses:

EXEC SQL INCLUDE SQLCA END-EXEC.

### 14.3 Cursors

COBOL:

EXEC SQL

DECLARE C1 CURSOR FOR SELECT ...

END-EXEC.

PL/I:

EXEC SQL DECLARE C1 CURSOR FOR SELECT ...;

EXEC SQL OPEN C1;

EXEC SQL FETCH C1 INTO :VAR1, :VAR2;

EXEC SQL CLOSE C1;

Behavior is similar, but:

* PL/I host variable typing is stronger
* PL/I error handling is more flexible

## Chapter 15 — Built-in Function Reference (EXTENDED)

PL/I has one of the richest built-in function sets of any traditional language.

Here are the major categories.

### 15.1 String Functions

| **Function** | **Description**              |
| ------------ | ---------------------------- |
| SUBSTR       | Extract substring            |
| INDEX        | Locate substring             |
| VERIFY       | Scan for unwanted characters |
| LENGTH       | Length of string             |
| TRIM         | Trim spaces                  |
| TRANSLATE    | Map characters               |
| REPEAT       | Repeat string                |

Examples:

LAST = SUBSTR(NAME, 6);

POS = INDEX(LINE, 'ERROR');

IF VERIFY(INPUT, '0123456789') > 0 THEN PUT SKIP LIST('Invalid digit');

### 15.2 Numeric Functions

* ABS
* MOD
* MAX
* MIN
* ROUND
* TRUNC
* CEIL / FLOOR
* FLOAT / FIXED
* RANDOM

Example:

P = MOD(A, B);

X = MAX(A, B, C);

### 15.3 Bit Functions

* BITOR
* BITAND
* BITXOR
* SHL / SHR (shift left/right)

### 15.4 Array Functions

* SUM
* MAX
* MIN
* MEAN
* SORT

Example:

TOTAL = SUM(SALES);

MAXVAL = MAX(SCORES);

COBOL requires loops for all these.

### 15.5 Condition Functions

Return information about exceptions:

* CONDITIONNAME
* CONDITIONINFO

### 15.6 Miscellaneous Functions

* DATE
* TIME
* SYSTEM
* ENVIRONMENT
* STORAGE
* ADDRESS OF
* ALLOCADDR

Example:

PUT SKIP LIST(DATE(), TIME());

## Chapter 16 — Advanced Data Features (OVERLAY, UNION, AREA)

PL/I includes powerful advanced features that COBOL programmers may find conceptually similar to REDEFINES or WORKING-STORAGE overlays, but far more flexible.

### 16.1 UNION (Advanced REDEFINES)

PL/I unions allow different fields to share the same memory.

Equivalent COBOL:

05 A PIC 9(4).

05 B REDEFINES A PIC X(4).

PL/I:

DCL 1 U UNION,

2 A FIXED BIN,

2 B CHAR(4);

Differences:

| Feature | COBOL REDEFINES | PL/I UNION |
|---------------------|------------------|============|
| Memory overlap | Yes | Yes |
| Type checking | None | Type checking for non-union members
| Nesting | Limited | Fully supported |
| Struct members | No | Yes |
| Controlled lifetime | No | Yes |

Union members share the same storage area.
Useful for:

* interpreting binary data
* overlaid numeric/string forms
* manual parsing of complex records

### 16.2 OVERLAY

PL/I’s overlay allows you to align structures or fields at exact offsets.

Example:

DCL 1 HEADER,

2 LENGTH FIXED BIN(31),

2 TYPE FIXED BIN(7),

2 FLAGS OVERLAY(LENGTH) BIT(8);

This allows reading a binary field and also treating its bits individually.

COBOL’s REDEFINES is the closest equivalent, but PL/I’s overlay is more precise.

### 16.3 AREA

An AREA is a region of memory that can contain dynamic objects.

Example:

DCL REGION AREA(1024);

DCL BUFFER CHAR(80) BASED(P);

ALLOCATE BUFFER IN(REGION);

P-> = 'HELLO';

Benefits:

* memory isolation
* managed allocation scope
* efficient bulk cleanup
* used in complex systems and parsers

COBOL has no equivalent.

### 16.4 STORAGE Class

Rarely used, but important in system-level PL/I:

DCL X CHARACTER(10) STORAGE;

Allows raw memory manipulation (like assembler).

## Chapter 17 — Concurrency and Tasking

PL/I supports **tasking**, a feature COBOL does not have.

### 17.1 TASK Statements

PL/I tasks allow concurrent execution within the same program.

Example:

TASK1: TASK; CALL PROCESS\_A; END TASK1;

TASK2: TASK; CALL PROCESS\_B; END TASK2;

CALL WAIT;

Capabilities:

* spawn multiple tasks
* wait for completion
* synchronize tasks
* share or isolate data

Used in:

* telecommunication systems
* high-speed data processing
* monitoring applications

COBOL has **no native concurrency**.

### 17.2 Event Handling

PL/I supports asynchronous events:

ON EVENT(READY) CALL HANDLER;

Used for:

* I/O availability
* signals
* inter-task communication

COBOL requires OS-specific APIs for asynchronous work.

## Chapter 18 — Debugging Techniques and ON Conditions

COBOL programmers typically rely on:

* DISPLAY
* IBM Debug Tool
* TRACE
* Abend-AID / Fault Analyzer

PL/I integrates debugging more deeply into the *language itself*.

### 18.1 ON ERROR for Debugging

Example:

ON ERROR BEGIN;

PUT SKIP LIST('Error occurred at:', CONDITION());

END;

Useful for:

* trapping run-time errors
* logging issues
* graceful recovery

### 18.2 ON UNDEFINEDFILE, ON FINISH

ON UNDEFINEDFILE BEGIN; ... END;

ON FINISH BEGIN; ... END;

These provide cleanup logic similar to FINALLY.

### 18.3 Built-in Debugging Functions

* CONDITION() — name of error
* CONDITIONINFO() — data about reason
* STORAGE() — memory info
* ENVIRONMENT() — system info

These have no COBOL equivalents.

### 18.4 Compiler Options for Debugging

Common options:

* LIST — listing with interleaved source and code
* XREF — cross-reference listing
* MAP — memory map
* OPTIONS(DEBUG) — insert debug code
* OPTIONS(OPTIMIZE) — enable optimization

These options often appear in:

* IBM Enterprise PL/I
* IBM z/OS PL/I
* AIX PL/I

## Chapter 19 — Performance Guidelines

PL/I’s rich features must be used carefully to avoid performance pitfalls.

### 19.1 Use FIXED BINARY Whenever Possible

Binary arithmetic is faster than decimal.

Use:

FIXED BIN(31)

Instead of:

FIXED DEC(7,2)

when fractions are not required.

### 19.2 Avoid Excessive POINTER and BASED Use

Pointers are powerful but can degrade readability and performance.

Use structures with STATIC or AUTOMATIC storage where possible.

### 19.3 Use VARYING Strings for Performance

Fixed CHAR strings are padded; VARYING is more efficient.

### 19.4 Avoid Unnecessary ON-units

ON-units impose overhead.
Use sparingly for real exceptional events.

### 19.5 Inline Arithmetic (Expression-Oriented)

PL/I allows expressions inside assignments:

RESULT = (A + B) \* (C - D) / E;

COBOL often requires separate intermediate fields.

Complex expressions reduce:

* temporary variables
* code size
* memory footprint

### 19.6 Compiler Optimization

Use:

OPTIONS(OPTIMIZE(FULL))

for production builds.

## Chapter 20 — Migration Strategies from COBOL to PL/I

This chapter presents real-world guidance on migrating COBOL logic into PL/I.

### 20.1 Translate Control Flow First

Replace:

* PERFORM → PL/I DO
* EVALUATE → PL/I SELECT
* MOVE → Assignment =

### 20.2 Translate Data Structures

Convert COBOL records to PL/I structures.

COBOL:

01 EMP.

05 ID PIC 9(5).

05 NAME PIC X(20).

PL/I:

DCL 1 EMP,

2 ID FIXED BIN(31),

2 NAME CHAR(20);

### 20.3 Replace COPY Libraries with %INCLUDE

* COPY → literal replacement
* %INCLUDE → PL/I preprocessor include

### 20.4 Convert File Logic

COBOL:

READ INFILE AT END MOVE 1 TO EOF.

PL/I:

ON ENDFILE(INFILE) EOF = 'Y';

READ FILE(INFILE) INTO(INREC);

### 20.5 Convert String Handling

Replace:

* STRING → ||
* UNSTRING → SUBSTR / INDEX
* INSPECT → VERIFY / TRANSLATE

### 20.6 Handling COMP-3 Fields

PL/I supports:

* PACKED
* BINARY
* DECIMAL

Conversions required depending on COBOL layout.

### 20.7 Testing and Validation

* Compare record counts
* Validate numeric fields
* Validate key fields
* Use ON ERROR logging during migration
* Regression test batch reports

## Chapter 21 — Idiomatic PL/I for COBOL Programmers

Examples of PL/I patterns that express logic more simply than COBOL.

### 21.1 Whole-Array Operations

SUMVAL = SUM(SALES);

COBOL requires a loop.

### 21.2 Whole-Structure Assignment

EMP2 = EMP1;

COBOL: multiple MOVE statements.

### 21.3 Selective Exception Handling

ON ZERODIVIDE ...;

COBOL: no equivalent.

### 21.4 Dynamic Buffers

ALLOCATE BUFFER;

Impossible in COBOL.

## Chapter 22 — Common Pitfalls for COBOL Programmers

### 22.1 Uninitialized AUTOMATIC Variables

Automatic variables are NOT automatically set to zeros/spaces.

COBOL WORKING-STORAGE initializes everything.

Solution:

DCL VAR FIXED BIN INIT(0);

### 22.2 Precision Errors

Binary fractions in FIXED BIN can produce rounding differences.

Use FIXED DEC when exact decimal precision required.

### 22.3 Pointer Misuse

Pointer errors cause:

* traps
* storage violations
* undefined behavior

Avoid BASED unless required.

### 22.4 Overreliance on ON-units

Do not use ON ERROR to mask logic problems.

### 22.5 VARYING String Length

String length matters:

DCL S CHAR(20) VARYING;

S = 'A';

/\* length=1, not space-filled \*/

COBOL programmers often assume trailing spaces.

## Chapter 23 — Comprehensive COBOL → PL/I Feature Equivalence Matrix

This chapter is an essential reference for any programmer migrating logic between the two languages.

It provides a complete, detailed mapping of COBOL constructs to their PL/I equivalents.

### 23.1 Program Structure

| **COBOL**               | **PL/I**                   |
| ----------------------- | -------------------------- |
| IDENTIFICATION DIVISION | PROC OPTIONS(MAIN)         |
| DATA DIVISION           | DCL statements anywhere    |
| PROCEDURE DIVISION      | Procedure body             |
| Paragraph               | Procedure or labeled block |
| Section                 | Not used                   |
| COPY                    | %INCLUDE                   |
| EXIT PROGRAM            | RETURN                     |
| STOP RUN                | END main procedure         |

### 23.2 Data Types

| **COBOL PIC** | **PL/I Type**    |
| ------------- | ---------------- |
| PIC X(n)      | CHAR(n)          |
| PIC 9(n)      | FIXED DEC(n,0)   |
| PIC 9(n)V99   | FIXED DEC(n+2,2) |
| COMP          | FIXED BIN        |
| COMP-3        | PACKED DECIMAL   |
| COMP-1/COMP-2 | FLOAT            |
| OCCURS        | Array            |
| REDEFINES     | UNION / OVERLAY  |

PL/I has additional capabilities beyond COBOL:

* POINTER
* BIT
* CHARACTER VARYING
* Multi-dimensional arrays
* Dynamic memory (CONTROLLED/BASED)

### 23.3 Control Flow

| **COBOL**        | **PL/I**     |
| ---------------- | ------------ |
| PERFORM UNTIL    | DO UNTIL     |
| PERFORM VARYING  | DO loop      |
| IF … THEN … ELSE | IF THEN ELSE |
| EVALUATE         | SELECT WHEN  |
| EXIT PARAGRAPH   | LEAVE        |
| NEXT SENTENCE    | ITERATE      |
| GOBACK           | RETURN       |

### 23.4 File I/O

| **COBOL Operation** | **PL/I Equivalent**   |
| ------------------- | --------------------- |
| READ INFILE         | READ FILE(INFILE)     |
| WRITE OUTFILE       | WRITE FILE(OUTFILE)   |
| OPEN INPUT          | OPEN FILE(INFILE)     |
| OPEN OUTPUT         | OPEN FILE(OUTFILE)    |
| OPEN I-O            | OPEN FILE with UPDATE |
| CLOSE file          | CLOSE FILE(file)      |
| AT END              | ON ENDFILE(file)      |
| INVALID KEY         | ON ERROR(file)        |

### 23.5 Strings

| **COBOL**              | **PL/I**                    |
| ---------------------- | --------------------------- |
| STRING                 | ( concatenate by using      |
| UNSTRING               | SUBSTR, INDEX               |
| INSPECT                | VERIFY, TRANSLATE           |
| Reference modification | SUBSTR(string,start,length) |

### 23.6 Arithmetic

| **COBOL**     | **PL/I**         |
| ------------- | ---------------- |
| COMPUTE A =   | A =              |
| ADD/SUBTRACT  | A = A + B        |
| ROUNDED       | ROUND(A)         |
| ON SIZE ERROR | ON FIXEDOVERFLOW |

### 23.7 SQL

| **COBOL**                | **PL/I**                   |
| ------------------------ | -------------------------- |
| EXEC SQL                 | EXEC SQL                   |
| INTO :WS-FIELD           | INTO :PLIVAR               |
| SQLCA in WORKING-STORAGE | DCL SQLCA LIKE SQLCA\_DEF; |

Fundamentally identical, but PL/I’s host variables are strongly typed.

### 23.8 Error Handling

| **COBOL**             | **PL/I**             |
| --------------------- | -------------------- |
| AT END                | ON ENDFILE           |
| INVALID KEY           | ON ERROR             |
| Declaratives          | ON condition         |
| No general exceptions | Full exception model |

### 23.9 Modularity

| **COBOL**                    | **PL/I**                         |
| ---------------------------- | -------------------------------- |
| CALL "name" USING vars       | CALL name(vars)                  |
| No nested routines           | Nested procedures                |
| No recursion                 | Full recursion                   |
| Parameters BY REFERENCE only | BY VALUE, BY REFERENCE, OPTIONAL |

### 23.10 Memory Model

| **COBOL**         | **PL/I**          |
| ----------------- | ----------------- |
| WORKING-STORAGE   | STATIC            |
| LOCAL-STORAGE     | AUTOMATIC         |
| LINKAGE           | Parameters        |
| No pointers       | POINTER           |
| No dynamic memory | CONTROLLED, BASED |

## Chapter 24 — Migration Checklist (Production-Ready)

This is a complete checklist used by professional teams when converting COBOL systems to PL/I or maintaining mixed environments.

### 24.1 Data Structure Migration Checklist

* Convert each COBOL record to a PL/I structure
* Convert PIC to PL/I fixed/decimal types
* Map COMP/COMP-3 correctly
* Convert REDEFINES to UNION/OVERLAY
* Convert OCCURS to PL/I arrays
* Replace COPYBOOKs with %INCLUDE files

### 24.2 Control Flow Checklist

* Replace PERFORM-loops with DO-loops
* Replace EVALUATE with SELECT WHEN
* Replace IF logic with equivalent PL/I logic
* Replace EXIT PARAGRAPH with LEAVE
* Replace NEXT SENTENCE with ITERATE

### 24.3 String Handling Checklist

* Replace STRING with ||
* Replace UNSTRING with SUBSTR + INDEX
* Replace INSPECT with VERIFY/TRANSLATE
* Replace reference modification with SUBSTR

### 24.4 File Handling Checklist

* Replace FD with FILE declaration
* Replace READ with READ FILE
* Replace WRITE with WRITE FILE
* Replace AT END with ON ENDFILE(file)
* Replace INVALID KEY with ON ERROR(file)
* Ensure file record structure matches buffer length

### 24.5 SQL Migration Checklist

* Declare host variables via DCL
* Convert PIC types to PL/I types
* Copy SQLCA definition correctly
* Validate cursor loops
* Adjust decimal type scale/precision

### 24.6 Exception Handling Checklist

* Add ON ERROR handlers
* Add ON ZERODIVIDE where needed
* Add ON SIZE/ON FIXEDOVERFLOW
* Add ON UNDEFINEDFILE for safety
* Do not overuse ON-units (use sparingly)

### 24.7 Best Practice Checklist

* Use FIXED BIN for counters and loop indexes
* Use VARYING strings for performance
* Avoid unnecessary POINTER use
* Keep procedures small and modular
* Use OPTIONS(OPTIMIZE) for production builds
* Use ON UNITS only for true exceptional conditions

## Chapter 25 — Professional Glossary (COBOL → PL/I)

This glossary provides working definitions of all important terms, written specifically for COBOL developers.

### 25.1 A–C

**ALLOCATE** — PL/I statement that creates dynamic memory (no COBOL equivalent).
**AREA** — PL/I memory pool for dynamic allocation.
**AUTOMATIC** — PL/I storage class equivalent to COBOL LOCAL-STORAGE.
**BASED** — PL/I object that exists only through a POINTER.
**BIT** — PL/I binary string data type.
**CALL** — invokes a PL/I or COBOL routine; equivalent to COBOL CALL.
**CHAR** — PL/I character string type.

### 25.2 D–H

**DCL** — PL/I declaration keyword (equivalent to DATA DIVISION entries).
**DO** — PL/I looping construct (equivalent to COBOL PERFORM loops).
**EDIT** — formatted output control.
**ENDFILE** — PL/I condition raised on EOF (COBOL AT END).
**ERROR** — PL/I condition for I/O or runtime errors.
**FIXED** — PL/I numeric type (binary or decimal).
**FREE** — releases CONTROLLED storage.
**GOTO** — jump statement (avoid, same as COBOL GO TO).

### 25.3 I–Q

**INDEX** — PL/I substring search function.
**INIT** — initializes variable value.
**ITERATE** — skip to next loop iteration (COBOL NEXT SENTENCE approximate).
**KEYED** — PL/I keyed file access (COBOL indexed file).
**LEAVE** — exit a loop or block (COBOL EXIT PARAGRAPH).
**LIKE** — structure/type-copy operator (similar to using a COPY record).
**ON-units** — PL/I exception handlers.

### 25.4 R–Z

**REPEAT** — string repetition function.
**SELECT WHEN** — PL/I version of EVALUATE.
**SIGNAL** — raises a condition (no COBOL equivalent).
**STATIC** — PL/I storage class equal to WORKING-STORAGE.
**STRUCTURE** — PL/I hierarchical record definition.
**SUBSTR** — extract substring.
**TRANSLATE** — character mapping function.
**UNION** — memory overlay (like REDEFINES).
**VARYING** — dynamic-length strings.

## Chapter 26 — Full Alphabetical Index

This section replicates the style of IBM Redbooks and professional reference manuals.
Only a selection is shown here due to size; the final DOCX will contain all entries.

**A**

* ALLOCATE (dynamic memory)
* AREA storage
* AUTOMATIC storage
* Arrays (PL/I)
* Arrays (COBOL OCCURS)

**C**

* CALL statement
* CHARACTER types
* CONTROLLED storage
* COPY → %INCLUDE

**D**

* DATA TYPES (COBOL vs PL/I)
* DECLARE (DCL) statements
* DO-loop semantics

**E**

* EDIT format
* ENDFILE condition
* EVALUATE → SELECT WHEN

**F**

* FILE declarations
* FIXED BIN
* FIXED DEC

**G**

* GOTO
* GRAPHIC strings

**I**

* INDEX function
* INSPECT replacement

**L**

* LEAVE
* LIKE structures

**M**

* MOVE → assignment
* MEMORY model

**O**

* OCCURS → arrays
* ON-units
* OVERLAY

**P**

* PARAMETERS (BY VALUE/REFERENCE)
* POINTER type
* PROCEDURES
* PICTURE vs DECIMAL types

**R**

* READ FILE
* REDEFINES → UNION

**S**

* SELECT WHEN
* SIGNAL
* SQL host variables
* STORAGE classes

**T**

* TASKING
* TRANSLATE
* TRIM

**U**

* UNDEFINEDFILE
* UNIONS

**V**

* VARYING strings
* VERIFY

**Z**

* ZERODIVIDE

## Chapter 27 — Final Professional Recommendations

1. **Understand PL/I’s power**: it is closer to C or Ada than to COBOL.
2. **Avoid unnecessary pointer programming** unless required.
3. **Use strong typing** (FIXED BIN, FIXED DEC) to ensure predictable arithmetic.
4. **Use ON-units judiciously**, not as normal control flow.
5. **Migrate step-by-step**, starting with:
   * data structures
   * loops
   * conditions
   * strings
   * I/O
6. **Prefer VARYING strings** for performance.
7. **Read compiled listings** (LIST, XREF) to understand generated code.
8. **Benchmark frequently**—PL/I’s optimization options matter.
9. **Modularize your code** using nested procedures.
10. **Use whole-structure and whole-array operations** where possible.

## Literature links:

## [IBM Enterprise PL/I for z/OS - IBM Documentation](https://www.ibm.com/docs/en/epfz/6.2.0)

[**Open PL/I Language Reference Manual**](https://www.microfocus.com/documentation/enterprise-developer/ed60/ED-VS2017/BKPFPFPREF.html)

[**Open PL/I User's Guide**](https://www.microfocus.com/documentation/enterprise-developer/ed60/ED-VS2019/BKPUPUPREF.html)