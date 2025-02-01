# Go Race Condition Example

This repository demonstrates a common concurrency bug in Go: a race condition caused by multiple goroutines accessing and modifying a shared variable without proper synchronization.

The `bug.go` file contains the buggy code. Running it will likely produce an output less than 1000, as goroutines may overwrite each other's updates to the `count` variable.

The `bugSolution.go` file provides a corrected version using a mutex to protect the shared variable.