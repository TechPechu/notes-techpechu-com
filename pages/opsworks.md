- Only opsworks stack is in scope of exam
- you write cookbooks in chef and get the application created
- Opswork manages your underneath instances
	- Timebased instances:
		- Opswork can auto bring instances as per schedule time
	- Load based instances:
		- We can configure to bringup instances based on the load
	- 24/7
		- Runs all the time
- Apps
	- We map the source code of your application, and we can get it deployed on our instances
- Stacks lifecycle events #exam-revise
  collapsed:: true
	- Setup
		- Happens whenever instance is booted
	- Configure
		- ![image.png](../assets/image_1654113059027_0.png)
	- Deploy
		- Deploy the application overall in all instances
	- Undeploy
		- Delete an app in the instances
	- Shutdown
		- To terminate the instances
- Autohealing
	- If any layer failed then it autoheal