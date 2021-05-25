### :beginner: Programs to Install

- Install **[Java JDK](https://www.oracle.com/br/java/technologies/javase/javase-jdk8-downloads.html)** in your computer;
- Install **[Java JRE](https://docs.oracle.com/goldengate/1212/gg-winux/GDRAD/java.htm#BGBFJHAB)** in your computer;
- Install **[Gradle](https://gradle.org/install/)** in your computer;
- Install **[Android Studio](https://developer.android.com/studio)** in your computer;

### Programs Configuration

:warning: If you already configured the programs, just go to **Env Variables Configuration**.

- **Gradle**

Create a new directory `C:\Gradle` with File Explorer.

Open a second File Explorer window and go to the directory where the Gradle distribution was downloaded. Double-click the ZIP archive to expose the content. Drag the content folder `gradle-<VERSION>` to your newly created `C:\Gradle folder`.

- **Android Studio**

After Android Studio installetion, open it and then go to `Configure > SDK Manager`.

Then, go to `SDK Tools` and download:
    - **Android SDK Build-Tools**
    - **Android SDK Command-line Tools**
    - **CMake**
    - **Android Emulator** (OPTIONAL)
    - **Android SDK Platform-Tools**
    - **Google USB Driver**


### :pencil: Env Variables Configuration

- Android Studio:
```
Name: ANDROID_HOME
Path: C:\Users\<USER>\AppData\Local\Android\Sdk
```

- Java Development Kit:
```
Name: JAVA_HOME
Path: C:\Program Files\Java\<JDK_VERSION>
```

- Java Runtime Environment:
```
Name: JRE_HOME
Path: C:\Program Files\Java\<JRE_VERSION>
```

- OS Path:
```
~ C:\Program Files\Java\<JDK_VERSION>\bin
~ C:\Gradle\<GRADLE_VERSION>\bin
~ C:\Users\<USER>\AppData\Local\Android\Sdk\platform-tools
~ C:\Users\<USER>\AppData\Local\Android\Sdk\build-tools\<VERSION>
```

*By [Névio Costa Magagnin](https://www.linkedin.com/in/n%C3%A9vio-magagnin-045710177/)*