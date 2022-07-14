# Streaming-Data-Demo

This demo will show how mule apps can utilize streaming to process large files that
may exceed allocated heap memory.  The demo takes a large xml file of students from an input
folder and breaks out information about each student individually to an output folder.

Streaming Documentation:

	https://docs.mulesoft.com/dataweave/2.4/dataweave-streaming

Setup:

You will need to modify the File Config element in the global.xml to whatever output/input
folders you would like to use.  The file used in this demo can be found here:



When running this demo locally, you can modify the runtime arguments to utilize less
memory than the size of the test file.  This will demonstrate and prove the app is streaming.
You can do this with the "-xms" and "-xmx" arguments (ex: -Xms512m -Xmx512m)
