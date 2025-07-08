# A Kernel Seedling
Programmed a kernel module written in C to count the number of processes running on the computer, as well as python unit tests.

## Building
```shell
make
sudo insmod proc_count.ko
```

## Running
```shell
cat proc/count
```
Sample Result: 136

## Cleaning Up
```shell
sudo rmmod proc_count
make clean
```

## Testing
```python
python -m unittest
```
Ran 3 tests successfully in 27.064 seconds.

```shell
uname -r -s -v
```
Module tested on Linux 5.14.8-arch1-1 kernel release version.

Credit: Assigment created by Professor Peter Reiher from UCLA.
