# Dart JSON Decoding Error

This repository demonstrates a common error in Dart when working with JSON APIs:  failure to handle potential `FormatException` exceptions that can arise from `jsonDecode`.  The `bug.dart` file contains code that can throw a `FormatException`, while `bugSolution.dart` shows how to handle this error gracefully.

## Reproducing the Bug

1. Run `bug.dart`. 
2. If the API returns an invalid JSON structure, observe that the program crashes with a `FormatException`.

## Solution

The `bugSolution.dart` demonstrates a robust solution by incorporating a `try-catch` block to handle the potential `FormatException`. This prevents unexpected crashes and allows for graceful error handling, enhancing the resilience of the application.