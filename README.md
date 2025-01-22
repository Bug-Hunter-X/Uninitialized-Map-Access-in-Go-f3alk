# Uninitialized Map Access in Go

This repository demonstrates a common error in Go: attempting to access an element of a map before it has been initialized.  Uninitialized map access will result in a runtime panic.

## The Bug

The `bug.go` file contains the erroneous code.  It declares a map `myMap`, attempts to assign a value to it, and then immediately tries to access that value without first initializing the map.  This will cause a runtime panic.

## The Solution

The `bugSolution.go` file shows the corrected code. The map is explicitly initialized using `make()` before any access attempts.