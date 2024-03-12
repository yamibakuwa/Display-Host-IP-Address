# Host Information Retrieval Script

This Python script allows you to retrieve the hostname and IP address of your local machine using the `socket` module.

## Prerequisites

- Python installed on your system.

## How it works

1. **Importing the `socket` module**: 
   The `socket` module in Python provides access to the BSD socket interface. This interface is commonly used for networking and communication purposes.

2. **Retrieving Hostname**: 
   The `socket.gethostname()` function returns the standard host name for the local machine. This is typically the fully qualified domain name.

3. **Retrieving IP Address**: 
   The `socket.gethostbyname()` function takes a hostname as input and returns the corresponding IP address. In this case, we pass the hostname retrieved in the previous step using `socket.gethostname()`.

4. **Displaying Host Information**:
   We print out the hostname and IP address obtained using the functions described above.

## Code Snippet

```python
import socket

print('Host name:', socket.gethostname())
print('Host IP address:', socket.gethostbyname(socket.gethostname()))

Host name: your-host-name
Host IP address: your-ip-address


Host name: your-host-name
Host IP address: your-ip-address
## Usage

    Open a Python environment (such as Jupyter Notebook).
    Copy and paste the code snippet into your Python environment.
    Execute the script to see your host name and IP address printed in the output.
