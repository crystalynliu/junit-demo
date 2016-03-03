##JUnit Demo

---

通过一个demo来演示JUnit在用命令编译java的使用方法

###**Step 1:clone the repository**

>git clone git@github.com:crystalynliu/junitDemoByTextEditor.git

---

###**Step 2:enter the folder**

>cd junitDemoByTextEditor

---

###**Step 3:Compile Caclculator.java**

>javac Calculator.java

The Java compiler creates a file `Calculator.class`.

---

**###Step 4:Compile CaclculatorTest.java**

On Linux or MacOS

>javac -cp .:junit-4.XX.jar CalculatorTest.java

and on Windows

>javac -cp .;junit-4.XX.jar CalculatorTest.java

The Java compiler creates a file `CalculatorTest.class`.

---

###**step 5:Run the test**

Run the test from the command line. On Linux or MacOS

>java -cp .:junit-4.XX.jar:hamcrest-core-1.3.jar org.junit.runner.JUnitCore CalculatorTest

and on Windows

>java -cp .;junit-4.XX.jar;hamcrest-core-1.3.jar org.junit.runner.JUnitCore CalculatorTest

###**step 6:The output is**

>JUnit version 4.12
.
Time: 0,006
OK (1 test)

The single . means that one test has been run and the OK in the last line tells you that your test is successful.

