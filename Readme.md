Steps to Execute the Script:
Step 1: Ensure that you have the required software and dependencies installed on your machine (e.g., Java Development Kit, Java 8).
Step 2: download the source code from the attachment.
Step 3: Open the project in your preferred Java development environment (e.g., Eclipse, IntelliJ IDEA).
Step 4: Set the local path of the Excel file in the application.properties file. If needed, update other configuration properties as well. - optional step
Step 5: Build the project to generate the executable JAR file. - build command (mvn clean install) or right click on your project Run as -> Maven Clean -> Maven Install (if you encountered jdk is rather than jre issue change the build path of your JDK right click -> build path -> configure build path -> Libraries -> JRE 8 -> Edit -> Alternate JRE choose JDK 1.8)
Step 6: Open the terminal or command prompt and navigate to the directory where the JAR file is located. (mostly jar will locate in target folder)
Step 7: Execute the JAR file using the following command:
java -jar automation-services-0.0.1-SNAPSHOT.jar {excel file path} {base folder path} {manage.service.path} {manage.service.apiproxy.path} 
 Note: The {excel file path} and {base folder path} are optional arguments. If not provided, the values will be fetched from the application.properties file.
 excel file path} - complete path of the created excel file 
 base folder path - where the path of the conf file is going to create
 ex: java -jar automation-user-0.0.1-SNAPSHOT.jar /Users/jensoncruz/Documents/TechM/Project/Optus/all_users/All_Phases_Service_Name.xlsx /Users/jensoncruz/Documents/TechM/Project/Optus/all_users/consolidated-users-services-1.1.198/pet/consolidated-users-services.ldif /Users/jensoncruz/Documents/TechM/Project/Optus/all_users/
Step 8: Follow the instructions displayed in the console to interact with the script and process the Excel sheet.