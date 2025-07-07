# A Kernel Seedling
Uses for_each_process to count processes currently running on the machine and prints the total.

## Building
To build the module, run this command in the same directory as the make file
```shell
make
```

## Running
Insert the module into the kernel with this command
```shell
sudo insmod proc_count.ko
```
Then run the kernel module to see the number of processes running using this command
```shell
cat /proc/count
```
Results:
138

## Cleaning Up
To clean up the binary that we created use this command
```shell
make clean
```
To remove module from the kernel use this command
```shell
sudo rmmod proc_count
```

## Testing
To test the program using a python script, use this command
```python
python -m unittest
```
Results:
```
...
---------------------
Ran 3 tests in 17.026s

OK
```

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.
This command outputs the kernel release version
```shell
uname -r -s -v
```
Results:
Linux 5.14.8-arch1-1 #1 SMP PREEMAT Sun, 26 Sep 2021 19:36:15 +0000
