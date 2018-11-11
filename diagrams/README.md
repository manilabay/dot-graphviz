
## How to convert dot code to graph

### Using Docker convert container
You could use [my another repo](https://github.com/manilabay/docker-graphviz-png-cli) to build a docker container convert tool, so you dont need to install dependencies and reuse it.

Once you have the tool image built you could run:
```console
cat input.dot | docker run -v your-host-path-or-Volume:/aws-icons --rm -i graphv
iz-convert-png > output.png
```

### Using dot command

```console
dot -Tpng input.dot > output.png
```

As a example to create the diagram for the mt-logical-architecture you must run:

```console
dot -Tpng mt-logical-architecture.dot > mt-logical-architecture.png
```
