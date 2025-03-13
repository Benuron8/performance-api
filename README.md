# performance-api

Performance testing an API:
	Concurrent users
	Short Peak Handling
	Sustained Load
	

Prerequisites:
Install Apache JMeter
Java (JDK 8 or later) installed and added to Path
Clone this repository or download the .jmx test plan

Test Scenarios

1. Concurrent Users Test
	Threads: 100
	Ramp-up: 20 sec
	Duration: 600 sec
	Simulates users joining gradually and staying active.
	
2. Peak Load Test
	Threads: 500
	Ramp-up: 30 sec
	Duration: 300 sec (5 min)
	Simulates sudden high traffic to check system limits.
	
3. Sustained Load Test
	Threads: 100
	Ramp-up: 120 sec
	Duration: 1800 sec (30 min)
	Tests long-term stability under continuous load.


How to run the tests:

Open jmeter in (GUI Mode):
Open the folder and run the jmeter.bat file
Click File and Open and select the jmx file
Click Start button to run.

By Default I only left the "Thread Group 2: Short Peak Handling" enable so only this test will run.
If you want to run the others, enable/disable the tests (using right click on the Thread Group.

To analyze the logs:
Options > Log viewer checked
