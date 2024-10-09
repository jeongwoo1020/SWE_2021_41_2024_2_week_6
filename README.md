# SWE_2021_41_2024_2_week_6

# Week 4 Assignment

* Link of your repository
[Repository Link](@jeongwoo1020)

```python
def isHappy(n):
  while True:
    sum = 0
    for i in range(len(str(n))):
      sum += int(str(n)[i]) ** 2
    if sum == 1:
      return True
    elif sum == 4:
      return False
    n = sum
```

* Description of your code
This function checks if a given number n is a "happy number", takes an integer n as input and enters a while True loop./
If the sum equals 4, it returns False, meaning the process will enter an unhappy number cycle and will never reach 1.

>> isHappy(19) => True/
>> isHappy(2) => False 
---

# Week 5 Assignment

```bash
>> docker exec <your_container> cat /etc/os-release
```
>> * This command executes the cat /etc/os-release command inside the running Docker container to display information about the operating system. The output will include details like the OS name, version, and ID.
<br>

```bash
>> docker exec <your_container> git --version
```
>> * This command shows the installed version of Git within the Docker container by running git --version. It ensures that Git is installed and displays its version number.
<br>
### Command 3
```bash
>> docker exec <your_container> python3 --version
```
>> * This command outputs the version of Python 3 installed inside the Docker container. It ensures that Python 3 is available and provides version information.
<br>
```bash
>> docker inspect --format="{{ .HostConfig.Binds }}" <container_name>
```
>> * This command inspects the Docker container configuration to check the volume bindings (if any) by using a specific format to filter the Binds information. This helps you see which directories from the host are mounted inside the container.
