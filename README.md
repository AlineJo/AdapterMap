> ### This is a simple Google map App. Using HMS Converter, I created an adpter map that should be able to work on both android devices and Huawei devices which doesn't have google play services.

> # Things you need to change in-order for this app to work:

####  1. update ` agconnect-services.json ` file. found under app folder (you need to change to project mode to see it. Otherwise, use finder/file explorer).

####  2. update `applicationId` in `build.gradle(app)` and enter your project package name instead. 

   
    android {
    compileSdk 30

    defaultConfig {
        applicationId "com.josephali.adaptermap" //change this to your project package! 
        minSdk 21
       ...
        
    }

    buildTypes {
       ...
    }
    compileOptions {
        sourceCompatibility JavaVersion.VERSION_1_8
        targetCompatibility JavaVersion.VERSION_1_8
    }
}

