This program constructs binary search trees with concurrent access. This is coded in and java 7 is required to run this program.

How to run:

	Copy all the .java and .sh files provided in the zip file to your home directory on the Tacc machine or whereever you are going to run the program from.

	Make sure all .java files and .sh file are in the same folder.
	
	The program accepts 5 parameters.
	number of instructions (constant at 1 million as suggested by professor but you can change this)
	key space size(number of keys in the tree)

	distribution type (1 for read-dominated, 2 for mixed and 3 for write-dominated)
	
	Number of threads

	implementation type (1 for coarse grained and 2 for fine grained)
  

    To run the program for 1 data point for fine grained approach, you need to run the compile.sh bash file as shown below:
	
	compile.sh <number of instructions> <key space size> <distribution type> <number of threads> <implementation type>

	eg: compile.sh 1000000 10000 2 16 2

    The program will output the throughput after averaging through 10 runs.


	Sample output:

	c557-504.stampede(9)$ compile.sh 1000000 10000 2 16 2
	Throughput : 3279.360524697684
	c557-504.stampede(10)$
