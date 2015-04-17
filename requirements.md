1. There should be a method on Calculator called "add" that takes a string representation of a number ("1") and returns it as a number (1).

2. When I give the method an empty string (""), it should return 0.

3. When I give the method a string containing two numbers delimited by a comma, it should return the sum of those numbers. For example, “2,3” or “2, 3” should return 5.

1. The method should handle an unknown amount of numbers delimited by commas and return their sum.

1. Allow the method to handle newlines as delimiters as well as commas (e.g “1\n2,3” should return 6).

1. Calling the method with a negative number should raise an ArgumentError with a message that says “negatives are not allowed” and the argument that was passed. If there were multiple negatives passed, include them all in the error message. For example, if someone passes “1,-2,-3”, the error message should say “negatives are not allowed (-2, -3)”.

    This is how you assert that an exception was raised in minitest. This is not the exact test you will be writing, you will need to change some things:

    ``` ruby
    error = assert_raises RuntimeError do
      some_expression_that_raises_exception
    end
    assert_equal "custom error message", error.message
    ```

1. Numbers bigger than 1000 should be ignored. For example, “1001,2” would just return 2. “1000,2” would return 1002.

1. Calling code should be able to specify a delimiter by passing an extra argument. For example I should be able to call the method like this: add(“1+2+3”, delimiter: “+”).

1. When I pass a custom delimiter, the previous delimiters (comma and new line) should still be valid. For example, add(“1,2+3\n4”, delimiter: “+”) should return 10.
