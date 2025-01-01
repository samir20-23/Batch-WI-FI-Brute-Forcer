<div id="badges" align="center">

[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=63CF15&lines=Wi-Fi+Brute+Forcer;Batch+Wi-Fi+Brute+Force+Tool)](https://git.io/typing-svg)

</div>

---

# Batch Wi-Fi Brute Forcer  
An active attack tool utilizing Batch commands to interact with Wi-Fi networks via CMD.

This program demonstrates how Batch files can be used to create a functional Wi-Fi network interaction tool. It showcases the use of built-in Windows CMD utilities for scanning networks, selecting targets, and attempting password combinations using a wordlist.

---

## **Features**
- **Interface Initialization**:  
  Automatically detects available wireless interfaces. If multiple interfaces are found, the user can select one.  
  - Command: `interface` (to manage and re-select the interface).  

- **Network Scanning**:  
  Enumerates all available Wi-Fi networks from the selected interface and lists them for selection.  
  - Command: `scan` (to scan for networks).

- **Custom Wordlist Support**:  
  Allows the user to specify a custom wordlist file for password attempts. A default wordlist is provided in the repository.  
  - Command: `wordlist <path_to_file>` (to set a custom wordlist).

- **Attack Execution**:  
  Attempts to connect to the selected Wi-Fi network using each password from the wordlist.  

- **Connection Counter**:  
  Tracks the number of connection attempts and increases the counter dynamically if association/authentication is detected.  
  - Command: `counter <value>` (to customize the number of queries).

- **Result Logging**:  
  If the attack is successful, the result (network name and password) is saved to `result.txt`.  

---

## **Usage Instructions**

### 1. Interface Initialization:
- On program execution, the wireless interface is automatically detected.  
- If there are multiple interfaces, the user will be prompted to choose one.  
- To change the interface later, use the `interface` command.

### 2. Scanning for Networks:
- Use the `scan` command to enumerate available networks.  
- Each network will be displayed with an associated number.  
- Choose the desired network by entering its number. Hidden networks (labeled "No Name") cannot be selected.

### 3. Selecting a Wordlist:
- The program includes a default wordlist file, but custom wordlists can be specified.  
- Use the `wordlist` command followed by the absolute or relative path to the file.

### 4. Executing the Attack:
- Use the `attack` command to initiate the process. The program will test each password from the wordlist against the selected network.  
- The program dynamically adjusts the connection counter to ensure a reliable connection check.

### 5. Adjusting the Counter:
- The counter controls how many connection attempts are made for each password. Default value: **10**.  
- Use the `counter` command to modify the value.

### 6. Viewing Results:
- Successful attacks are logged in the `result.txt` file, storing the SSID and corresponding password.

---

## **Commands**
| Command     | Description                                  |  
|-------------|----------------------------------------------|  
| `help`      | Displays the help screen.                   |  
| `wordlist`  | Specify a custom wordlist file.             |  
| `scan`      | Performs a Wi-Fi network scan.              |  
| `interface` | Manage and select the Wi-Fi interface.      |  
| `attack`    | Executes the attack on the selected network.|  
| `counter`   | Sets the number of connection attempts.     |  
| `exit`      | Exits the program.                          |  

---

## **Limitations**
- Works on **Windows 10** and **Windows 11** only.  
- Only supports network names (SSIDs) with **ASCII characters**.  
- Cannot attack hidden networks.  
- Performance may be slow due to its reliance on the `netsh` utility.  

---

## **Contributors**
- **TheKvc**  
- **Ankitamehra93**  
- **lioen-dev**  
- **akshatbhatter1**  

Special thanks to **TheBATeam** and **AACINI** for their support.

---

For more projects, visit: [TechnicalUserX GitHub](https://github.com/TechnicalUserX)

Press any key to continue...

---
 