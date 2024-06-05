# Ject: A Simple and Effective Way to Describe System Behavior

- **Version**:[[1.2.3]](.ject)

Ject is a collection of UML-like diagrams that provide a simple and effective way to describe the behavior of a system. These diagrams are designed to be easy to understand and can be used to document the behavior of a system in a concise and clear way.

## Ject Diagrams

There are several different types of Ject diagrams, each with its own specific purpose. These diagrams can be identified by their starting and ending characters, as shown in the table below:

---
| Diagram | Start | End | Description |
|:--|:-:|:-:|:--|
| Ejection | `[Eject(Node="target")]` | `Void` | Represents the removal of a node from the system. |
| Adjection | `'start'` | `'end'` | Represents the addition of a new node to the system. |
| Objection | `"start"` | `"end"` | Represents the creation of a new object in the system. |
| Subjection | `[start]` | `[end]` | Represents the creation of a new subject in the system. |
| Rejection | `(start)` | `(end)` | Represents the rejection of input based on a specific condition. |
| Injection | `:start` | `;end` | Represents the injection of data into the system. |
| Conjection | `'start` | `end'` | Represents the making of a conjecture based on assumptions and confidence. |
| Interjection | `<start` | `>end` | Represents the interjection of data into the system with a specific operation. |
| Projection | `{start}` | `}end` | Represents the projection of data into a specific dimension and coordinate system. |
| Trajection | `~start` | `end` | Represents the trajectory of data over a specific time period and trajectory type. |
---

### Ject in Action

Here is an example of how Ject diagrams can be used to describe the behavior of a simple system:

This diagram shows the ejection of a node named "target" from the system. The input to the "target" node is shown on the left, and the next node that will be connected after the ejection is shown on the right.

```E.ject
[Eject(Node="target")]
    target --> [Eject] --> Void
    ^                      |
    |                      V
   Previous node         Next node
   (Input to "target")    (Connected after "target")
```

An Adjection can be identified by start=`'`, and optional end=`'`.

```Ad.ject
              +---------+
              | NewNode |
              +---------+
                   |
                   V
    +----------+   |   +-----------+
    | Previous +-->+-->+ Next node |
    |  node    |       |           |
    +----------+       +-----------+
```

An Objection can be identified by start=`"`, and end=`"`.

```Ob.ject
Object: CustomObject
{
    Properties:
        Property1: Type1
        Property2: Type2
        ...

    Methods:
        Method1(Parameter1: Type1, Parameter2: Type2): ReturnType1
        Method2(Parameter1: Type1): ReturnType2
        ...

    Events:
        Event1
        Event2
        ...
}
```

A Subjection can be identified by start=`[`, and end=`]`.

```Sub.ject
Subject: CustomSubject
{
    State: CurrentState

    Properties:
        Property1: Type1
        Property2: Type2
        ...

    Methods:
        RegisterObserver(Observer: ObserverType): Void
        RemoveObserver(Observer: ObserverType): Void
        NotifyObservers(): Void
        ...

    Observers:
        Observer1: ObserverType
        Observer2: ObserverType
        ...
}
```

A Rejection can be identified by start=`(`, and optional end=`)`.

```Re.ject
[Reject(Criteria: ConditionType)]

Input --> [Reject] --> Output
```

An Injection can be identified by start=`:`, and optional end=`;`.

```In.ject
[Inject(Data: AnyType)]

Input --> [Inject] --> Output
```

A Conjection can be identified by start=```, and end=```.

```Con.ject
[Conject(Assumptions: AssumptionType, Confidence: Double)]

Input --> [Conject] --> Output
```

An Interjection can be identified by start=`<` or start=`>`, and optional end=`>`.

```Inter.ject
[Interject(Data: AnyType, Operation: OperationType)]

Input --> [Interject] --> Output
```

A Projection can be identified by start=`{`, and end=`}`.

```Pro.ject
[Project(Data: AnyType, Dimensions: Integer, CoordinateSystem: SystemType)]

Input --> [Project] --> Output
```

A Trajection can be identified by start=`~`.

```Tra.ject
[Traject(Data: AnyType, TimeSteps: Integer, TrajectoryType: Type)]

Input --> [Traject] --> Output
```

## Details

Let me provide you with a more detailed explanation of the functionalities of the classes in the .jectCalibrator program:

1. .jectCalibrator:
   - This class serves as the main entry point for the program.
   - It is responsible for initializing and configuring the necessary components, such as the .jectSettings, .jectParser, and .jectCompiler.
   - The Calibrate() method is used to load default settings, check for a settings file, and configure the Parser, Compiler, and other dependencies based on the loaded settings.

2. .jectParser:
   - This class handles the parsing of the file content.
   - It utilizes the .jectSettings and .jectAST (Abstract Syntax Tree) properties.
   - The Configure() method updates the Settings property.
   - The Parse() method tokenizes the file content into a list of tokens and builds the AST based on these tokens.

3. .jectCompiler:
   - This class is responsible for compiling the AST into executable code.
   - It relies on the .jectSettings, .jectAST, and CompiledCode properties.
   - The Configure() method updates the Settings property.
   - The Compile() method traverses the AST and generates the compiled code based on the nodes.

4. .jectFormatter:
   - This class handles the formatting of the compiled code.
   - It utilizes the .jectSettings and FormattedCode properties.
   - The Configure() method updates the Settings property.
   - The Format() method applies formatting rules to the compiled code based on the settings.

5. .jectTester:
   - This class is responsible for running tests on the system components.
   - It relies on the .jectSettings property and maintains a list of .jectTestResult objects.
   - The Configure() method updates the Settings property.
   - The RunTests() method executes each test case using the configured system components, compares the expected output with the actual output, and adds the test result to the list of results.

6. .jectPerformanceAnalyzer:
   - This class analyzes the performance of the system components.
   - It utilizes the .jectSettings property and maintains a dictionary of execution times.
   - The Configure() method updates the Settings property.
   - The AnalyzePerformance() method records the start time, processes the test case using the configured system components, and records the execution time.

7. .jectDebugger:
   - This class facilitates the debugging of the system components.
   - It has a property for .jectSettings.
   - The Configure() method updates the Settings property.
   - The Debug() method creates a debugger UI, processes the test case with debugging enabled, and displays the debug results and the final output code.

8. .jectErrorHandler:
   - This class handles errors that occur during the processing of the code.
   - It has a property for .jectSettings.
   - The Configure() method updates the Settings property.
   - The HandleErrors() method processes the test case using the configured system components, checks for errors in the processed code, and returns a list of errors.

I have found the following issues:

1. The .jectCalibrator class should implement the IDisposable interface to properly dispose of any unmanaged resources it uses.

2. The .jectParser class constructor should accept the .jectSettings instance as a parameter and use it to configure the parser.

3. The .jectCompiler class constructor should accept the .jectSettings instance as a parameter and use it to configure the compiler.

4. The .jectFormatter class constructor should accept the .jectSettings instance as a parameter and use it to configure the formatter.

5. The .jectTester class constructor should accept the .jectSettings instance as a parameter and use it to configure the tester.

6. The .jectPerformanceAnalyzer class constructor should accept the .jectSettings instance as a parameter and use it to configure the performance analyzer.

7. The .jectDebugger class constructor should accept the .jectSettings instance as a parameter and use it to configure the debugger.

8. The .jectErrorHandler class constructor should accept the .jectSettings instance as a parameter and use it to configure the error handler.

9. The .jectParser class should implement the IParser interface and expose a method to parse a string.

10. The .jectCompiler class should implement the ICompiler interface and expose a method to compile an AST.

11. The .jectFormatter class should implement the IFormatter interface and expose a method to format compiled code.

12. The .jectTester class should implement the ITester interface and expose methods to run tests and compare output.

13. The .jectPerformanceAnalyzer class should implement the IPerformanceAnalyzer interface and expose methods to analyze performance.

14. The .jectDebugger class should implement the IDebugger interface and expose methods to debug test cases.

15. The .jectErrorHandler class should implement the IErrorHandler interface and expose methods to handle errors.

These classes work together to provide functionalities such as calibration, parsing, compiling, formatting, testing, performance analysis, debugging, and error handling in the .jectCalibrator program.

## Usage

To use Ject diagrams in your documentation, simply copy and paste the diagram into your markdown file. You can then customize the diagram by changing the values of the nodes and edges.

## Caution

Ject diagrams are designed to be simple and easy to understand. They are not meant to replace traditional UML diagrams, but rather to complement them. Ject diagrams are best used to describe the behavior of a system in a concise and clear way.

### Benefits of Using Ject

There are several benefits to using Ject diagrams to describe system behavior:

-**Simple and easy to understand:** Ject diagrams are designed to be simple and easy to understand, even for people who are not familiar with UML diagrams.
-**Concise and clear:** Ject diagrams can be used to describe the behavior of a system in a concise and clear way.
-**Versatile:** Ject diagrams can be used to describe a wide variety of system behaviors.

### Conclusion

Ject is a simple and effective way to describe system behavior. Ject diagrams are easy to understand and can be used to document the behavior of a system in a concise and clear way. If you are looking for a way to improve the documentation of your system, Ject is a great option to consider.
