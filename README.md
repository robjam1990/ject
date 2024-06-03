# Ject

Ject is a collection of UML-like diagrams that describe the behavior of a system. Each diagram is a single word followed by a colon and a description of the diagram. The diagrams are designed to be simple and easy to understand. They can be used to describe the behavior of a system in a concise and clear way.

## Diagrams

An Ejection can be identified by initiate=`;`.

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

These classes work together to provide functionalities such as calibration, parsing, compiling, formatting, testing, performance analysis, debugging, and error handling in the .jectCalibrator program.

## Usage

To use Ject diagrams in your documentation, simply copy and paste the diagram into your markdown file. You can then customize the diagram by changing the values of the nodes and edges.

## Caution

Ject diagrams are designed to be simple and easy to understand. They are not meant to replace traditional UML diagrams, but rather to complement them. Ject diagrams are best used to describe the behavior of a system in a concise and clear way.
