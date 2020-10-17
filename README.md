### This is forked repo of ifogsim(https://github.com/Cloudslab/iFogSim)

# iFogSim
A Toolkit for Modeling and Simulation of Resource Management Techniques in Internet of Things, Edge and Fog Computing Environments

## How to initialize project ?

* Create a Java project in Eclipse. 
* Inside the project directory, initialize an empty Git repository with the following command
```
git init
```
* Add the Git repository of iFogSim as the `origin` remote.
```
git remote add origin https://github.com/DongDongJu/iFogSim
```
* Pull the contents of the repository to your machine.
```
git pull origin master
```
* Include the JARs (except the CloudSim ones) to your Eclipse project.  

## How to export JAR file

### eclipse

1. right click on your project

2. click export-java-Runnable JAR file

3. check library handling method what you want

4. make sure your JAR file path

## How to run example 

1. go to src/org/fog/test/perfeval

2. run example files in there with JAVA

## Get Result using file

*   check src/org/fog/utils/Config class
*   you can get result as csv file format. 
*   if you run with MultiClassApp.java with file output then, you can get below results, (set FILE_OUTPUT option in config file)
```
	Total execution time	,
	Average Latency of Control Loop (application Loop),
    	Energy Consumption[cloud],
    	Energy Consumption[fog-layer],
    	Energy Consumption of each device,	
    	Total network usage
```

## Get Result by using terminal
*   requirement : java8
*   export your sample app as jar type (ex jars/ifogsim_arr.jar)
*   run with config file (ex configs/*.config)
*   run
```
	java -jar jars/ifogsim_two_layer.jar configs/4_test.config
```
*	then you can get result file where path in config file.


# References
1. Harshit Gupta, Amir Vahid Dastjerdi , Soumya K. Ghosh, and Rajkumar Buyya, <A href="http://www.buyya.com/papers/iFogSim.pdf">iFogSim: A Toolkit for Modeling and Simulation of Resource Management Techniques in Internet of Things, Edge and Fog Computing Environments</A>, Software: Practice and Experience (SPE), Volume 47, Issue 9, Pages: 1275-1296, ISSN: 0038-0644, Wiley Press, New York, USA, September 2017.

2. Redowan Mahmud and Rajkumar Buyya, <A href="http://www.buyya.com/papers/iFogSim-Tut.pdf">Modelling and Simulation of Fog and Edge Computing Environments using iFogSim Toolkit</A>, Fog and Edge Computing: Principles and Paradigms, Wiley Press, New York, USA, 2018 (in press).

