# Ject

Ject is a collection of UML-like diagrams that describe the behavior of a system. Each diagram is a single word followed by a colon and a description of the diagram. The diagrams are designed to be simple and easy to understand. They can be used to describe the behavior of a system in a concise and clear way.

## Diagrams

```E.ject
[Eject(Node="target")]
    target --> [Eject] --> Void
    ^                      |
    |                      V
   Previous node         Next node
   (Input to "target")    (Connected after "target")
```

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

```Re.ject
[Reject(Criteria: ConditionType)]

Input --> [Reject] --> Output
```

```In.ject
[Inject(Data: AnyType)]

Input --> [Inject] --> Output
```

```Con.ject
[Conject(Assumptions: AssumptionType, Confidence: Double)]

Input --> [Conject] --> Output
```

```Inter.ject
[Interject(Data: AnyType, Operation: OperationType)]

Input --> [Interject] --> Output
```

```Pro.ject
[Project(Data: AnyType, Dimensions: Integer, CoordinateSystem: SystemType)]

Input --> [Project] --> Output
```

```Tra.ject
[Traject(Data: AnyType, TimeSteps: Integer, TrajectoryType: Type)]

Input --> [Traject] --> Output
```

## Usage

To use Ject diagrams in your documentation, simply copy and paste the diagram into your markdown file. You can then customize the diagram by changing the values of the nodes and edges.

## Caution

Ject diagrams are designed to be simple and easy to understand. They are not meant to replace traditional UML diagrams, but rather to complement them. Ject diagrams are best used to describe the behavior of a system in a concise and clear way.
