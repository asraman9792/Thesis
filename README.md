# Thesis
* For power grid models, a corresponding GLM file needs to be placed
  in the `GLM/` directory in order to make topology visualization
  possible.
* For network devices, after adding a new device into the database the
  file `Scripts/NetGen.py` needs to be edited to make sure that the
  new device is integrated with the built-in network model.
* The built-in network model cannot be changed without modifying the
  source code; this filed needs to be edited
  `Scripts/NetGen.py` mentioned above.

# Installation

For  installation  GridAttack, follow the steps below to set up all the additional components:

* Install Tkinter, a Python binding to the Tk GUI toolkit, which was used to develop the GridAttack GUI:
* sudo apt-get install python3-tk
* Install the pip3 packet manager:
* sudo apt install python3-pip
* Install other packages required by GridAttackAnalyzer as specified in the file requirements.txt included with the distribution by running the following command from the GridAttack/ directory:
* sudo -H pip3 install -r requirements.txt


# Quick Start
Use a terminal window to navigate to the GridAttack directory, then start the GUI by running the command below:

python3 GridAttack.py
GridAttack GUI

Once the GUI is displayed, as shown above, follow the next steps to configure and run the analysis:
<img width="960" alt="image" src="https://user-images.githubusercontent.com/45739151/179213472-22ad2476-1460-4d67-ac65-2c8dc86eb4e4.png">



Select the input parameters: Smart Grid Model, Smart Meter Connection, CVEs, Devices and Vulnerabilities. The built-in network model is shown below; please consider it when selecting the devices to make sure that end-to-end routes exist.
<img width="573" alt="image" src="https://user-images.githubusercontent.com/45739151/179213508-2804cb66-cc9d-4574-8314-af6e679bef93.png">


Network Model

Click on the "Generate File" button to generate the initial attack analysis file; this file can be fine tuned if desired by:

Option 1: Click on "1 - Manual Edit" to open the file, then edit it directly.
Option 2: Use "Edit a Device & CVE" to select a specific device and assign a new CVE value to it, then click on "Update" to bring the attack analysis file up to date.
Click on the "Run" button to start the attack analysis.

When the attack analysis process finishes, you can use any of the following functions by clicking on the corresponding buttons:

Attack Graph: Show the computed attack graph
Graph Source File": Show the CSV file containing the attack graph data
Security Metrics: Show the CSV file containing the computed security metrics
Plot Metrics: Visualize the computed security metrics
