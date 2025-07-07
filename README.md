# A Kernel Seedling
Uses for_each_process to count processes currently running on the machine and prints the total.

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko

cat /proc/count
```
Results:
138

## Cleaning Up
```shell
make clean

sudo rmmod proc_count.ko
```

## Testing
```python
python -m unittest
```
Results: 
Run 3 tests in 17.026s
OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
Results:
Linux 5.14.8-arch1-1 #1 SMP PREEMAT Sun, 26 Sep 2021 19:36:15 +0000
