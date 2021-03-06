### :beginner: Programs to Install

- Install **[Java JDK](https://www.oracle.com/br/java/technologies/javase/javase-jdk8-downloads.html)** in your computer;
- Install **[Gradle](https://gradle.org/install/)** in your computer;
- Install **[Android Studio](https://developer.android.com/studio)** in your computer;
- Install **[Git](https://git-scm.com/downloads)** in your computer;

If you already configured the programs, just go to **[Env Variables Configuration](https://github.com/NEVI0/how-to-configure-mobile-environment#pencil-environment-variables-configuration)**.

### :small_orange_diamond: Gradle Configuration

Create a new directory `C:\Gradle` with File Explorer.

Open a second File Explorer window and go to the directory where the Gradle distribution was downloaded. Double-click the ZIP archive to expose the content. Drag the content folder `/gradle-<VERSION>` to your newly created `C:\Gradle` folder.

### :small_orange_diamond: Android Studio Configuration

After Android Studio installation, open it and then go to `Configure > SDK Manager`.

Then, go to `SDK Tools` and download:
- **Android SDK Build-Tools**
- **Android SDK Command-line Tools**
- **CMake**
- **Android Emulator** (OPTIONAL)
- **Android SDK Platform-Tools**
- **Google USB Driver**

### :small_orange_diamond: Git Configuration

If you want, you can follow step by step in this **[video](https://www.youtube.com/watch?v=7YVQLZp1jb0)**.

- First of all, generate a new SSH Key:
```
~ ssh-keygen -t rsa -b 4096 -C "<YOUR_GITHUB_EMAIL>"
```

The key is created in `C:\Users\<USER>\.ssh`. After just press **ENTER** for all steps.

In **GitHub**, go to `Settings > SSH and GPG Keys > New SSH Key`, provide a title for the key and **copy / paste (INTERE KEY)** your generated key in the field.

- Then, add your **GitHub** name and e-mail:
```
~ git config --global user.name "<GITHUB_NAME>"

~ git config --global user.email "<GITHUB_EMAIL>"
```

### :pencil: Environment Variables Configuration

For this configuration, go to `Update Operation System Environment Variables > Environment Variables > System Environments` and then:

- Create a new variable called **ANDROID_HOME** with the path of **Android SDK**: `C:\Users\<USER>\AppData\Local\Android\Sdk`
- Create a new variable called **JAVA_HOME** with the path of **Java JDK**: `C:\Program Files\Java\<JDK_VERSION>`
- Create a new variable called **JRE_HOME** with the path of **Java JRE**: `C:\Program Files\Java\<JRE_VERSION>`

Now, edit **Operation System Path Variable** and add the `/bin` folders of the programs:

- `C:\Program Files\Java\<JDK_VERSION>\bin`
- `C:\Gradle\<GRADLE_VERSION>\bin`
- `C:\Users\<USER>\AppData\Local\Android\Sdk\platform-tools`
- `C:\Users\<USER>\AppData\Local\Android\Sdk\build-tools\<VERSION>`

*By [N??vio Costa Magagnin](https://www.linkedin.com/in/n%C3%A9vio-magagnin-045710177/)*
