PrimeFinder
=================================================

![Points](../../blob/badges/points.svg)

For this homework, you will modify the work queue implementation such that it tracks and waits for pending work, eliminating the need for a "task manager" class. Then, your code should use it to find prime values.

## Hints ##

Below are some hints that may help with this homework assignment:

  - Add a `pending` variable to the `WorkQueue` class to track unfinished work and implement the `finish()` method to wait until there is no more pending work.

  - There should *not* be a `pending` variable or `TaskManager` nested class in the `PrimeFinder` class! You will need to create an inner "task" or "work" class, however.
  
  - Implement the multithreaded `findPrimes(int, int, int)` method in `PrimeFinder` using your modified `WorkQueue` class. There should be 1 task or `Runnable` object for each number being tested and the `run()` method of these objects should use the `isPrime(int)` method.
  
  - Do not try to use lambda expressions or streams for your initial approach.
  
These hints are *optional*. There may be multiple approaches to solving this homework.

## Instructions ##

Use the "Tasks" view in Eclipse to find the `TODO` comments for what need to be implemented and the "Javadoc" view to see additional details.

The tests are provided in the `src/test/` directory; do not modify any of the files in that directory. Check the run details on GitHub Actions for how many points each test group is worth. 

See the [Homework Guides](https://usf-cs272-spring2023.github.io/guides/homework/) for additional details on homework requirements and submission.
