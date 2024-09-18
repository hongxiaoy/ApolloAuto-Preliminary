# Creating

In this section, I will show a simple proto definition in Apollo.

```protobuf
syntax = "proto2";

package apollo.common;

message Point2D {
  optional double x = 1 [default = nan];
  optional double y = 2 [default = nan];
}
```
The `.proto` file starts with a package declaration, which helps to prevent naming conflicts between different projects. In C++, your generated classes will be placed in a namespace matching the package name, in this code it's `apollo.common`.
