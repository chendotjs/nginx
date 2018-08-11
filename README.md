## Usage

```
mkdir build
cd build
cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON -DCMAKE_BUILD_TYPE=Debug ..
make -j5
mkdir temp
mkdir logs
./nginx -c ../nginx.conf -p . -t  # do not run, just check.
./nginx -c ../nginx.conf -p .
```

`auto_index_module` is used. `index` module has some problem.
