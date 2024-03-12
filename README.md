# Host Information Retrieval Script

This Python script allows you to retrieve the hostname and IP address of your local machine using the `socket` module.

## Prerequisites

- Jupyter Notebook installed on your system.

## How it works

1. **Importing the `socket` module**: 
   The `socket` module in Python provides access to the BSD socket interface. This interface is commonly used for networking and communication purposes.

2. **Retrieving Hostname**: 
   The `socket.gethostname()` function returns the standard host name for the local machine. This is typically the fully qualified domain name.

3. **Retrieving IP Address**: 
   The `socket.gethostbyname()` function takes a hostname as input and returns the corresponding IP address. In this case, we pass the hostname retrieved in the previous step using `socket.gethostname()`.

4. **Displaying Host Information**:
   We print out the hostname and IP address obtained using the functions described above.

## Usage

1. Open a Python environment (such as Jupyter Notebook).
2. Copy and paste the code snippet into your Python environment.
3. Execute the script to see your hostname and IP address printed in the output.

## Code Snippet

```python
import socket

print('Host name:', socket.gethostname())
print('Host IP address:', socket.gethostbyname(socket.gethostname()))


```
## Output

```python
Hostname: your-host-name
Host IP Address: your-ip-address

```
