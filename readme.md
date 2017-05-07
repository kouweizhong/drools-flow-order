# Working with reverse order :(

HumanFlow -> Rule Flow below like this
![](https://preview.ibb.co/dRcdMQ/Human_Flow.png)

- StepA and StepA1 are in ruleflow-group "A"
- StepB and StepB1 are in ruleflow-group "B"
- StepC and StepC1 are in ruleflow-group "C"

HumanInit just call the flow like this

```java
$ kcontext.getKieRuntime().startProcess("test.HumanFlow");
```

# but working reverse order C -> B -> A

![](https://image.ibb.co/i57TMQ/console.png)
# excepted that A -> B -> C

Note: Drools Latest final version: 6.5.0.Final
