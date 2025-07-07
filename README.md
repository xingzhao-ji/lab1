# A Kernel Seedling
TODO: intro
Adds /proc/count; reading it uses for_each_process to count processes and prints the total.

## Building
```shell
TODO: cmd for build
make
```

## Running
```shell
TODO: cmd for running binary
sudo insmod proc_count.ko

cat /proc/count

sudo rmmod proc_count
```
TODO: results?
138

## Cleaning Up
```shell
TODO: cmd for cleaning the built binary
make clean
```

## Testing
```python
python -m unittest
```
TODO: results?
results: Run 3 tests in 17.026s
OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
TODO: kernel ver?
Linux 5.14.8-arch1-1 #1 SMP PREEMAT Sun, 26 Sep 2021 19:36:15 +0000
