# LogginLab

See comments in LogginLab class for instructions.

### Only use logging for output.

Always using `System.out.println()` is a beginner habit.
Sure, it's handy, but just dumping debugging info into what's known as `standard out` & `standard error` isn't something
you will find you can do when you start making code that ends up in __production__.
There is a much more common means of getting output, when debugging or logging, and that is to use a `Logger`.

### What's logging?

Java logging is a built-in feature that allows developers to output messages to a log file or console for debugging and status output. It provides a way to track the flow of an application and identify issues that may arise.

Java logging has several levels of severity, including INFO, WARNING, and SEVERE, which can be used to categorize messages based on their importance. Developers can also create their own custom log levels if needed.

To use Java logging, developers can create a Logger object and use its methods to log messages. The Logger object can be configured to output messages to a file, console, or other output stream.

Java logging also supports logging exceptions, which can be helpful in identifying the cause of an error. Developers can log the stack trace of an exception to help pinpoint where the error occurred.

Overall, Java logging is a powerful tool for debugging and monitoring the status of an application.

### Notice this in the LogginLab class

```java
import java.util.logging.Level;
import java.util.logging.Logger;

public class LogginLab {
    private final static Logger logger = Logger.getLogger(LogginLab.class.getName());

// and so on...
```

What *are* thos imports for??

### What you need to do

- Write a method called `thresholdReached`, returns true if argument 'limit' is over the threshold.
- use `thresholdExceeds` for a pattern.
- Write a test for the method in the Test class.
- tests are *important*. Get in the habit of writing one or more for each `method`.
