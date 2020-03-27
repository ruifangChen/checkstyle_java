load("@checkstyle_java//checkstyle:checkstyle.bzl", "checkstyle_test")

checkstyle_test(
  name = "HelloWorld-checkstyle",
  target = "HelloWorld",
)
java_library(
  name = "greeter",
  srcs = ["Greeter.java"],
)

java_library(
  name = "hello_world",
  srcs = ["HelloWorld.java"],
  deps = [":greeter"],
)

java_binary(
  name = "HelloWorld",
  main_class = "example.HelloWorld",
  runtime_deps = [":hello_world"],
)


