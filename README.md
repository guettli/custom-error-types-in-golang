# Custom Error Types in Golang


https://www.reddit.com/r/golang/comments/14ye8c3/errorsas_and_custom_errors_with_value_receiver/



Start: errors.As() does not work as expected.


errors.Is() is for checking for sentinel error values. It's great, use it.

errors.As() checks for error types. It is like a "cast" in other languages. Avoid it, except you need to access fields of the custom error.

...
