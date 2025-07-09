###### **JavaFX Prim's MST Visualizer**



A JavaFX application to visualize Prim’s Minimum Spanning Tree (MST) step by step.



---



######  **Features**



\- Interactive visualization of Prim's algorithm.

\- Step-by-step construction of the MST.

\- Easy-to-follow UI for educational purposes.



---



######  **Requirements**



**Java Development Kit (JDK) 24**



Download: https://download.oracle.com/java/24/latest/jdk-24\_windows-x64\_bin.exe



 **JavaFX SDK 22**



Download: https://gluonhq.com/products/javafx/

Direct ZIP Download: https://download2.gluonhq.com/openjfx/22/openjfx-22\_windows-x64\_bin-sdk.zip



⚠ Important: JavaFX is NOT included in the JDK. You must download and configure it separately.



---



 **IntelliJ IDEA Setup**



Follow these steps carefully to configure your project:



---



**1) Create or Open Your Project**



\- Launch IntelliJ IDEA.

\- Create a new Java Project or open your existing project folder.



---



**2)Set Project SDK to JDK 24**



1\. Navigate to:

&nbsp;  File > Project Structure > Project

2\. Set Project SDK to JDK 24.

3\. If JDK 24 is not listed:

&nbsp;  - Click Add SDK.

&nbsp;  - Browse to your JDK installation folder.

&nbsp;  - Example path:

&nbsp;    C:\\Program Files\\Java\\jdk-24



---



**3) Extract JavaFX SDK**



1\. Download the JavaFX SDK ZIP.

2\. Extract it to a folder, for example:

&nbsp;  C:\\javafx-sdk-22

3\. Verify you see a lib directory inside the extracted folder containing .jar files.



---



4\) **Configure VM Options**



These options tell Java where to find JavaFX libraries.



1\. Go to:

&nbsp;  Run > Edit Configurations

2\. Select your main class configuration or create a new Application configuration.

3\. Click Modify Options and check VM Options.

4\. In VM options, paste this line (replace <path-to-javafx-lib> with the actual path to the lib folder):



&nbsp;  --module-path "<path-to-javafx-lib>" --add-modules javafx.controls,javafx.fxml --enable-native-access=javafx.graphics



Example:



&nbsp;  --module-path "C:\\javafx-sdk-22\\lib" --add-modules javafx.controls,javafx.fxml --enable-native-access=javafx.graphics



---



**>>>Running the Application<<<**



After completing the setup:



\- Build the project.

\- Run your main class.

\- The JavaFX window should launch, displaying Prim’s MST visualizer.



---



**>>>How to Use<<<**



Add vertex: Click on the canvas to create nodes.



Connect vertices: Click one vertex, then another to connect; enter edge weight.



Select source vertex: Click a node to choose the starting point for Prim’s MST.



Remove node: Right-click a node, then select Remove Node to delete it.



Run Prim’s MST: Click the Run MST button to visualize the algorithm.











