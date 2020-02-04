Reference: https://www3.ntu.edu.sg/home/ehchua/programming/java/JavaNativeInterface.html

#Create HelloJNI.java   
#Compile it: javac -h . HelloJNI.java  
#Create HelloJNI.c  
#export JAVA_HOME=/your/java/installed/dir  
#Compile C program: gcc -fPIC -I"$JAVA_HOME/include" -I"$JAVA_HOME/include/linux" -shared -o libhello.so HelloJNI.c  
#Run the program: java -Djava.library.path=. HelloJNI  


That's it!
