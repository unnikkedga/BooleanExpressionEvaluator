BooleanExpressionEvaluator
===================

A boolean expression evaluator project using a Recursive Descent Parser and the Interpreter Pattern

You can find a description of the project [here](https://unnikked.ga/how-to-evaluate-a-boolean-expression)

## How to use

Clone the repository with: 

```
git clone https://github.com/unnikked/BooleanExpressionEvaluator.git
```

Compile:

```
javac src/tk/unnikked.booleanevaluator/*.java src/tk/unnikked/booleanevaluator/*/*.java src/tk/unnikked/booleanevaluator/ast/*/*.java
```

And execute it with (remember to `cd src`): 

```
java tk/unnikked/booleanevaluator/BooleanEvaluator
```

You can also pipe in a file using `-f` directive

```
cat yourfile | java java tk/unnikked/booleanevaluator/BooleanEvaluator -f
```

Here an execution example:

```
$ cat test | java tk/unnikked/booleanevaluator/BooleanEvaluator -f
(true & ((true | false) & !(true & false)))
AST: (true & ((true | false) & !(true & false)))
RES: true
```

##License

Check `LICENSE`