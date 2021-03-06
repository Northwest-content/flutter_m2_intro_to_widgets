Now, you are going to add a cat image inside the app 😻.

To display an image on the screen, you need to follow these steps:

1. Insert the image into the project folder:

   - Create a folder called **assets** in the root of your flutter project. These kinds of folders usually include some static data, like images, fonts, icons, etc.
   - Inside the **assets** folder, create another folder called **images**, which contains all images that will be used in your app.
   - Insert your image in the **images** folder.

   > Download the image from this [link](https://raw.githubusercontent.com/Northyoust-content/flutter_profile_page_app/main/assets/images/profile.png?token=AFZTMZMPTZSYHKF6DP5JOK3AVY5JY)

![screenshot](https://lh3.googleusercontent.com/q9z8pe0FK5HetzPBcSQfPC82p4DqgT2oQkpiapuLsz88XMTmBH_f0fX8arjJ8E7ChEzEStoS9hme-i6U4NoMGLvx5Lrunl-2fgIb6fYBv8Ds1hnlAnWk5rpJX1fr-OzvphlML1Pf)

2. Tell Flutter where the path of the image is. To do that, you need to edit the **pubspec.yaml** file, and add the path of your cat image.

> Note: when you add another new image, you will need to add its path below other images paths.

```yaml
assets:
  - assets/images/profile.png
```

3. Save the changes inside the **pubspec.yaml** file by clicking:
   - Windows: **Ctrl + S**
   - Mac: **Command + S**

> Note: When you save **pubspec.yaml**, the vscode will pop up the following dialogue

![screenshot](https://lh5.googleusercontent.com/279IAwnenB5NeEEXtFDFdHocHr_EGSds8cEP7Tg95gPqXKTYQ14O0Kw_bUHDmUXci4alRV-HmXHH4IcThXy-6aaFRCZI4Tulbv0bzPultstu4x76RfaFuoUM4SUVNUHFcXz7oX_K)

**Important**: when you edit the **pubspec.yaml** file, you will need to rerun the app.

4. Load the image using **Image.asset** widget, which helps you to render the image on the screen, by passing the path of the cat image as the first argument of that widget.

```dart
Scaffold(
     backgroundColor: Colors.orange,
     body: Image.asset(
       'assets/images/profile.png',
    ),
  );
```

![screenshot](https://lh3.googleusercontent.com/8YTTYo04fZZA-yzSqj_axwZ2nlinSXjtGGdY6MoALcLZROdwWxbzU_zPzzK-wKWGSzBHwnPkAU25403KhFaDhExgVlfevfP-stNvT9QBOdcn6OwnXZZUCmN6DO7gfjPRQDXFcp4x)

5. Resize the image using **width** and **height** properties inside the **image.asset** widget.

   ```dart
   Image.asset(
          'assets/images/profile.png',
          width: 200,   // <- here
          height: 200,  // <- here
       )
   ```
