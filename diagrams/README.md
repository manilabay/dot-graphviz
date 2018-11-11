
## How to convert dot code to graph

```console
dot -Tpng input.dot > output.png
```

As a example to create the diagram for the mt-logical-architecture you must run:

```console
dot -Tpng mt-logical-architecture.dot > mt-logical-architecture.png
```

## Using Docker container convertion

Use my another repo to build a graphviz convert docker container and run:

```console
cat file.dot | docker run -v your-volume:/aws-icons --rm -i graphviz-converter > file.png
```
