ShellPilot User Guide
=====================

Overview
--------

ShellPilot is a robust and user-friendly GUI application designed to streamline the automation of SSH command execution across multiple remote hosts. Built with a focus on efficiency and ease of use, it empowers system administrators, network engineers, and IT professionals to perform bulk operations effortlessly, eliminating the need for repetitive manual tasks.

Key features include:

* **Multi-host Management:** Manage and execute commands on a large number of servers using inventory files, accelerating administrative workflows.
* **Credential Handling:** Securely manage SSH credentials through dedicated credential files to ensure seamless authentication across hosts.
* **Concurrent Execution:** Leverages multi-threading capabilities to run commands simultaneously on multiple hosts, significantly reducing execution time.
* **Job Output and Reporting:** Collate and display command output per host, with options to generate detailed CSV or text reports for compliance and auditing.
* **Debug and Logging:** Enable debug logging for enhanced transparency and troubleshooting.
* **Intuitive Profile Management:** Save and reuse your configuration profiles for consistency and efficiency across sessions.

With its modern interface and comprehensive functionality, ShellPilot simplifies complex SSH automation tasks, helping you maintain control and visibility over your infrastructure from a central application.

![SSH terminal automation](ShellPilot_User_Interface.gif "SSH Automation Image")

Table of Contents
-----------------

* [Getting Started](#getting-started)
* [User Interface Overview](#user-interface-overview)
* [Profile Management](#profile-management)
* [Input Configuration](#input-configuration)
    * [Host Inventory File](#host-inventory-file)
    * [SSH Credential File](#ssh-credential-file)
    * [Command List File](#command-list-file)
* [Execution Control](#execution-control)
* [Viewing Output](#viewing-output)
* [Debug Logging](#debug-logging)
* [Saving and Loading Profiles](#saving-and-loading-profiles)
* [Troubleshooting](#troubleshooting)
* [Contact and Support](#contact-and-support)

Getting Started
---------------

* **Installation**: Download and install ShellPilot from the official repository or website.
* **Launching the Application**: Open the ShellPilot application by double-clicking the executable file.

User Interface Overview
-----------------------

The main window consists of several sections:

* **Top Bar**: Contains the menu button and license status.
* **Title Section**: Displays the application name, version, and developer information.
* **Profile Management Section**: Allows users to select, create, edit, and delete profiles.
* **Input Configuration Section**: Where users can specify input files and settings.
* **Output Frames**: Displays the status of hosts and job output.
* **Status and Progress**: Shows the current activity status and progress bar.
* **Debug Console**: Displays debug logs if enabled.

Profile Management
------------------

* **Creating a New Profile**: Click the "New Profile" button and enter a name for the profile.
* **Editing a Profile**: Select a profile from the dropdown and click "Edit Profile" to modify its settings.
* **Deleting a Profile**: Select a profile and click "Delete Profile" to remove it from the list.

Input Configuration
-------------------

### Host Inventory File

* **Purpose**: Contains a list of hosts (IP addresses or hostnames).
* **Format**: CSV file with a header row `Host_IP`.
* **Selection**: Click "Browse" next to the "Host Inventory File" field to select the file.

Example:
Host_IP
192.168.1.1
192.168.1.2
example.com

### SSH Credential File

* **Purpose**: Contains SSH credentials (username and password).
* **Format**: CSV file with headers `username`, `password`, and optionally `port`.
* **Selection**: Click "Browse" next to the "SSH Credential File" field to select the file.

Example:
username,password,port
admin,password123,22
user,securepass,22

### Command List File

* **Purpose**: Contains commands to be executed on the hosts.
* **Format**: CSV or text file with a header row `Control Command`.
* **Selection**: Click "Browse" next to the "Command List File" field to select the file.

Example:
Control Command
ls -l
df -h
uptime

Execution Control
-----------------

* **Starting Execution**: Click the "Start Scan" button to begin executing commands on the specified hosts.
* **Stopping Execution**: Click the "Stop Scan" button to halt the execution at any time.

Viewing Output
--------------

The output of executed commands is displayed in the "Job Output" section. Select a host from the "Host Status" tree view to view specific output related to that host.

Debug Logging
-------------

* **Enabling Debug Logging**: Check the "Enable Debug Log" box to activate debug logging.
* **Viewing Debug Logs**: The debug console will display logs related to the application's operations.

Saving and Loading Profiles
---------------------------

* **Saving Current Profile**: Click "Save Current Profile" to save the current settings into the active profile.
* **Loading Profiles**: Profiles are automatically loaded from the configuration file on startup.

Troubleshooting
---------------

* **Common Issues**:
    * **File Not Found**: Ensure the specified file paths are correct and the files exist.
    * **Invalid Format**: Check that the input files are formatted correctly as per the specifications.
    * **SSH Connection Errors**: Verify that the SSH credentials are correct and that the hosts are reachable.

Contact and Support
-------------------

For further assistance, contact the developer:

* **Name**: Rhythm Kr. Dasgupta
* **Email**: [www.linkedin.com/in/rhythmkrdasgupta/](mailto:www.linkedin.com/in/rhythmkrdasgupta/)

Conclusion
----------

ShellPilot is a powerful tool for managing SSH command execution across multiple hosts. By following this user guide, you can effectively utilize its features for automated compliance scanning and reporting. For any additional questions or support, please reach out to the developer.
