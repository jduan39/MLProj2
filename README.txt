
For this project I used ABAGAIL. 

Requirements: Refer to ABAGAIL GitHub for requirements https://github.com/pushkar/ABAGAIL 

Compile: Navigate to ABAGAIL directory and run "ant"

Then run java -cp ABAGAIL.jar tests.OptdigitsTest <# hidden layers> <# Training iterations> <rhc, sa, or ga>

Examples

java -cp ABAGAIL.jar tests.OptdigitsTest 1 1 rhc
java -cp ABAGAIL.jar tests.OptdigitsTest 1 10 sa 
java -cp ABAGAIL.jar tests.OptdigitsTest 1 100 ga
  


These output to different csvs that take the form <algorithmname>-train.csv and <algorithmname>-test.csv. The training file gets rewritten with each run, but the test file appends to the end of the file

To run the optimization problem tests run these commands

java -cp ABAGAIL.jar opt.test.NQueensTest
java -cp ABAGAIL.jar opt.test.MyTravelingSalesman
java -cp ABAGAIL.jar opt.test.MyKnapsackTest

These test also output to csvs that follow the form <problemname>_<algorithm>.csv
These csvs also get overwritten each run

