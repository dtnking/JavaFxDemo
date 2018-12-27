This is a demo project of how to use JavaFx 11 (include the libraries, modules and dependencies). The IDE I used in this project is IntelliJ by JetBrains which can be downloaded [here](https://www.jetbrains.com/idea/download/#section=windows).

I am using JDK 11 which you will need to include all the libraries, modules or dependencies needed manually whenever you use JavaFx. (Previous version had all of them within the SDK). Else, the following errors will be generated:<br/>

Without including the libraries:<br/>
 ![image4592](https://user-images.githubusercontent.com/26379432/50488052-a17a3600-0a3b-11e9-8de3-03167e5f5c25.png)

 Without including the modules:<br/>
 ![image4603](https://user-images.githubusercontent.com/26379432/50489358-2ec08900-0a42-11e9-93cc-3f780f98f464.png)

 The steps to include are as below:

###### 1. Include the libraries.</br>
You need to include all the libraries or else the packages can not be imported. Go to this [website](https://gluonhq.com/products/javafx/) to download JavaFx 11. Extract it into a folder of your own. Then open up IntelliJ, go to File->Project Structure->Global Libraries. Click the + and go to the folder where you have previously extracted the JavaFx 11. Go to Lib to select all the files inside except for src.zip and click OK -> OK.

 ![image4512](https://user-images.githubusercontent.com/26379432/50486992-70980200-0a37-11e9-9384-755cb70299c1.png)    

##### 2. Include the modules.<br/>
Now go to Run->Edit Configuration->Configuration and add this line in the VM options:<br/>
 ```--module-path C:/Users/user/Documents/javafx-sdk-11.0.1/lib --add-modules=javafx.controls,javafx.fxml```<br/>
 Replace C:/Users/user/Documents/javafx-sdk-11.0.1/lib with the path of your extracted JavaFx 11. Be aware to also replace \ to / of your path if you copy directly from your Quick Access from your folder.

 After the steps, the JavaFx 11 should be working now.
