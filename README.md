# Search-Event-nearby
The application will search for events located nearby and will assist in purchasing of ticket
Developer Instructions
I.	Steps to run the application
1.	Open the link and download the zip file
2.	Open the zip and copy the GridDevelop folder into your local machine
3.	Goto GridDevelop->GridDevelop->bin->Debug
4.	Run the GridDevelop.exe
5.	If the windows defender blocks the application, select more info and press run anyway
6.	Enter the x coordinate and y coordinate in the box next to labels x and y or select the available coordinates from the drop-down list. The user can enter any location (even outside the world)
7.	Press the Submit button
8.	The nearby events are displayed in the box below

II.	Steps to build
1.	Open the link and download the zip file.
2.	Make sure that your system has Visual Studio 2015 or higher. 
3.	Open the zip and open GridDevelop folder.
4.	Select the GridDevelop.sln file.
5.	Double click and open it in Visual Studio.
6.	Press the Start button on toolbar or press F5.
7.	The project will build and the application will start running.
III.	Assumptions
1.	The range of the coordinates of the events is between -10 to +10
2.	All the tickets for an event are priced same
3.	I have assumed that the price for each ticket is a whole number
4.	The maximum distance is assumed to be 1000 between user’s location and event locations
IV.	How might you change your program if you needed to support multiple events at the same location? 
I have written a function which detects events assigned by the random seed generator to the same location and fixes it by giving it an open location in the grid. So, I would need to remove that function and the program would support multiple events.
V.	How would you change your program if you were working with a much larger world size? 
I have used a grid which is of size 20*20. If it was a larger world I would need to replace it with n*m where n being the size of x-axis and m being the size of y-axis. The program is written in such a way that we can easily change it to our required world. If the world size is increased then the max value should also be increased from 1000.
