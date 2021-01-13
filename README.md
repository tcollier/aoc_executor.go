# AoC Golang Executor

Golang executor for the [Advent of Code Solver](https://github.com/tcollier/aoc_solver).

## Signature

```go
type Input interface{}

type solverFunc func(Input) string

func Executor(input Input, part1 solverFunc, part2 solverFunc, args []string)
```

## Template Code

```go
package main

import (
	"os"

	"aoc.com/tcollier"
)

func part1Answer(input tcollier.Input) string {
	return // the answer
}

func part2Answer(input tcollier.Input) string {
	return // the answer
}

func main() {
  var input = // load input
	tcollier.Executor(input, part1Answer, part2Answer, os.Args)
}
```
