For the following, let us assume this math expression:

```
x = sin(pi / 2)
```

TapDigit lexical scanner will produce:

| **Type** | **Value** |
|:---------|:----------|
| Identifier	| x         |
| Operator	| =         |
| Identifier	| sin       |
| Operator	| (         |
| Identifier	| pi        |
| Operator	| /         |
| Number	  | 2         |
| Operator	|  )        |

TapDigit parser will produce:

```
{
  "Expression": {
    "Assignment": {
      "name": {
        "Identifier": "x"
      },
      "value": {
        "Function": {
          "name": "sin",
          "args": [
            {
              "Binary": {
                "operator": "/",
                "left": {
                  "Identifier": "pi"
                },
                "right": {
                  "Number": "2"
                }
              }
            }
          ]
        }
      }
    }
  }
}
```