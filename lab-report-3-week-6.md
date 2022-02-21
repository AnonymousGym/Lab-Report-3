# Lab Report 3

__Step 1__

Copying the whole markdown-parse directory to the ieng6 account.

![Image][11]

[11]: 1.png

__Step 2__

Logging into the ieng6 account after doing this and compiling and running the tests for the repository.

![Image][12]

[12]: 2.png

![Image][16]

[16]: 6.png

__Step 3__

Combining scp, ;, and ssh to copy the whole directory and run the tests in one line.
First I deleted markdown-parse-1 from the server.
Then combine all codes as one line:
scp -r . yig017@ieng6.ucsd.edu:~/markdown-parse-1; ssh yig017@ieng6.ucsd.edu "cd markdown-parse-1; javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java;java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"

![Image][14]

[14]: 4.png

![Image][15]

[15]: 5.png
