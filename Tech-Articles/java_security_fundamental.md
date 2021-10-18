## Java Security Fundamental

## Understanding Java

The Java programming language originally came from the "Green Project" project of the American software company Sun Microsystems. The project was led by James Gosling, Patrick Naughton, Mike Sheridan and Bill Joy. Initially, the project was aimed at making smart devices. However, because they were not satisfied with the results of the C++ and C programming languages, they decided to create their own more complex programming language. Java is a programming language that is often used to develop software, Android applications, and the back-end parts of websites.

## Security in Java
1. Strongly Styled
Java has good security features, one of which is strongly type where the code we type must have a strong type in the sense that the variable we use or what we create must be declared the data type of the variable.
2. Bytecode Verification
The basic philosophy of Java is that it is inherently secure from the point of view that no user program can corrupt the host machine or improperly interfere with other operations on the host machine, and it is possible to protect certain trusted methods and data structures.
3. Runtime Type Safety Check
The process of verifying and enforcing type constraints – type checking – can occur either at compile time (static checks) or run time (dynamic checks). If the language specification requires strong typing rules (i.e., more or less only allows automatic type conversion that doesn't lose information), one can refer to the process as being strongly typed, otherwise,
 as weakly typed. These terms are not usually used in a strict sense.
4. Class Loaders
This feature is used to use other classes in Java, so there is no need to code repeatedly because one class can be used repeatedly
5. Security Managers
This feature is used to manage security in the Java programming language so that it can facilitate security and operation.

## Java Virtual Machine
1. Class Loaders
Class Loader reads the .class file, then generates binary data and stores it according to the method area. For each .class file
2. Linking
Linking consists of three stages, namely: Verification to ensure that the .class file has been properly checked, and that the file has been formatted and created correctly by the compiler. If the verification process fails, the runtime exception will run java.lang.VerifyError. Preparation or preparation is a process by which
The JVM allocates memory for class variables and initializes memory to default values. Resolution is the process of replacing a symbolic reference from a typed reference to a direct reference. The parsing process is done by searching the method area to find entity references.
3. Initialization
At this stage, all allocated static variables are initialized according to the values ​​specified in the program code and static blocks (if any). Processes run from top to bottom in the class hierarchy and from parent to child.

## Java Sandbox
Over time, Java improved the sandbox model and resulted in a better security architecture. Security support features are typically implemented through the Java Security API and mirrored by the java.security package. This package provides a set of classes and interfaces that are easy to configure. There is a Provider class that represents a Java security API provider, where the provider implements some or all of the Java security. The services provided by the provider include cryptographic algorithms, key generation, conversion and management facilities. The Massage Digest class is a class in its implementation that compares the message digest value with the original value. The java.security package implements message digest via the MessageDigest class. To generate message digest, we can use MD5 or SHA-1 algorithm.

## Java Sandbox Elements
1. Permissions
Permissions are special operations that the code is allowed to perform. Certain permissions (such as java.security.AllPermission, which allows code to perform any operation) do not require a name. Otherwise, the name is based on the permission type, for example, the file permission name is the file or directory name.
2. Keystores
Java code can be signed, which requires a digital certificate, such as jarsigner (or an equivalent program). You can grant permission for code signed by a specific entity.
3. Code sources
Code sources are a combination of codebase and signers. The signature field must match the alias listed in the keystore. The codebase can be any valid URL. Because they are URLs, codebases always use slashes to refer to things like addresses or directories

## Happy Learning!


[@zal-ghiffari](https://github.com/zal-ghiffari/)
