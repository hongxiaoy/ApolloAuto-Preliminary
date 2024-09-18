# Compiling

Now run the compiler, specifying the source directory (where your application’s source code lives – the current directory is used if you don’t provide a value), the destination directory (where you want the generated code to go; often the same as `$SRC_DIR`), and the path to your `.proto`.

```bash
protoc -I=$SRC_DIR --cpp_out=$DST_DIR $SRC_DIR/point.proto
```

This generates the following files in your specified destination directory:
- `point.pb.h`, the header which declares your generated classes.
- `point.pb.cc`, which contains the implementation of your classes.
