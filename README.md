# parallel-programing-java
This repo is to insert all files and codes of Parallel Programing in Java Couse  from Rice University.

	
	->Module One – Task Parallelism
	
	USING MAVEN!!!
		->Maven is a build tool which automatically manages dependencies, 
		source code compilation, test compilation, and test execution. 
		
		
->Using Maven
		Compiling with Maven from the Command Line
		(TERMINAL COMMAND)=-> mvn compile	
		
		
->Using JavaC
		Compiling Manually Using Javac
		If you wish to compile manually using the command line (without Maven), you will need to add the following JARs to your classpath while building both the provided source and test files using javac: hamcrest-core-1.3.jar, junit-4.12.jar, and pcdp-core-0.0.4-SNAPSHOT.jar. One possible way to invoke the javac command from the root folder is as follows:
	
	COMMAND:
		$ javac -cp ./hamcrest-core-1.3.jar:./junit-4.12.jar:./pcdp-core-0.0.4-SNAPSHOT.jar:target/classes/:target/test-classes/ src/main/java/edu/coursera/parallel/Setup.java src/test/java/edu/coursera/parallel/SetupTest.java
	
	
	
Lecture: Task Creation and Termination

Lecture: Creating Tasks in Java’s Fork/Join Framework

Lecture: Computation Graphs, Work, Span, Ideal Parallelism

Lecture: Multiprocessor Scheduling, Parallel Speedup

Lecture: Amdahl’s Law

Module One - Demonstration Videos
Lecture: ReciprocalArraySum using Async-Finish

Lecture: ReciprocalArraySum using RecursiveAction’s in Java’s Fork/Join Framework

Module One - Assignments
Quiz: Module 1 Quiz

Coding Mini Project 1: Reciprocal-Array-Sum using the Java Fork/Join Framework

	->
	

 
 
 Notes:
 	(Using one arrya to get the sum of this array using async process, we need to use the "Divide and conquer algorithm , that means
 	we need to divide the array to get (the Sum) of thease two parts .
 	Each sum will be "calculated" by one Core of your processor , this means:
 	Sum 1 -> It will be calculated by CORE 0
 	Sum2 -> It will be calculated by CORE 1 
 	
 	Examplification:
 	
 	Finsih{
 		Async{
 		sum1 = sum of lower half 
 		
 		sum2 = sum of upper half
 	
 	sumtotal= sum1+ sum 2
 	
 		->So after all sums get done, the finish will pass the result of the calcs to sumtotal to get the total value.
 			The 2 tasks will run async
 			 
 		->Java Fork-Join Framework
 		
 
 
 	
 
 
 
 
 
 
 
 
 
 

	->Module Two – Functional Parallelism
Lecture: Futures: Tasks with Return Value

Lecture: Futures in Java’s Fork/Join Framework

Lecture: Memoization

Lecture: Java Streams

Lecture: Data Races and Determinism

Module Two - Demonstration Videos
Lecture: ReciprocalArraySum using RecursiveTask's in Java's Fork/Join Framework

Lecture: Parallel List Processing Using Java Streams

Module Two - Assignments
Quiz: Module 2 Quiz

Coding Mini Project 2: Analyzing Students Statistics Using Java Parallel Streams

 

	->Module Three – Loop Parallelism
Lecture: Parallel Loops

Lecture: Parallel Matrix Multiplication

Lecture: Barriers in Parallel Loops

Lecture: One-Dimensional Iterative Averaging

Lecture: Iteration Grouping/Chunking

Module Three - Demonstration Videos
Lecture: Parallel Matrix Multiplication

Lecture: Parallel One-Dimensional Iterative Averaging

Module Three - Assignments
Quiz: Module 3 Quiz

Coding Mini Project 3: Parallelizing Matrix-Matrix Multiply Using Loop


	->Module Four – Data Flow Synchronization and Pipelining
Lecture: Split-phase Barriers with Java Phasers

Lecture: Point-to-Point Synchronization with Phasers

Lecture: One-Dimensional Iterative Averaging with Phasers

Lecture: Pipeline Parallelism

Lecture: Data Flow Computing

Module Four - Demonstration Videos
Lecture: Phaser Examples

Lecture: Pipeline & Data Flow Parallelism 

Module Four - Assignments
Quiz: Module 4 Quiz

Coding Mini Project 4:Using Phasers to Optimize Data-Parallel Applications
