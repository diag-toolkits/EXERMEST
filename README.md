## About EXERMEST ##

EXERMEST (Extracting Features and Correlating Resource Use Counters and Message Types) is an open-source inter-component error propagation and recovery diagnostic tool based on resource use data and message logs analysis.  It is developed using C++, Boost and R statistical libraries.  The tool uses a configuration file.  In the configuration file, the system administrator can specify: (i) the directory for resource use data matrix, (ii) the directory for message types data matrix, (iii) the names of resource use counters, (iv) the names of message types, and (v) the year for the data matrices.  When the tool is executed using the configuration file, it automatically executes the EXERMEST workflow and generates the feature extraction reports, correlation reports and graphs.  The reports can then be used by systems administrators to infer the cause of system problems.

## Obtaining EXERMEST ##
A 64-bit version compiled for Linux is available for downloading [here.](https://tinyurl.com/ybsxxeyl)  If you have an enquiry about the tool, feel free to get in touch with me. (Email: echuah@turing.ac.uk or edwardchuah@acm.org)

## Installing and executing EXERMEST ##
Download the zip file and unzip its content into a directory of your choice.  Add `[directory]/exermest/toolkit/DiagTK/Release` to the directory path in your favourite Linux shell.  Then, run the command `diagtk -generateCfgFile` which will create a configuration file.  An config-file with default name *cfgfile* will be generated.  The config-file contains a set of default parameters.  If you wish to change any of the parameters, simply use your favourite shell editor to change the default parameters.  To execute the EXERMEST workflow, run the command `diagtk -autorunEXERMEST [config-file]` where `[config-file]` is the name of the configuration file.  A user manual will be available soon.

## Acknowledgement ##
This research was supported by The Alan Turing Institute under the EPSRC, UK grant EP/N510129/1 and The Alan Turing Institute-Intel partnership,
