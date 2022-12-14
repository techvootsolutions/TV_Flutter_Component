# Component

Creating Flutter component.


## Installing

1.  Add dependency to `pubspec.yaml`

    *Get the latest version in the 'Installing' tab on [pub.dev](https://pub.dev/packages/flutter_components)*

```dart
  dependencies:
      flutter_components: <latest-version>
```

2.  Import the package
```dart
import 'package:flutter_components/flutter_component.dart';
```

# 1) Neumorphic Widgets

Screenshot | Screenshot | Screenshot
------------ | ------------- | -------------
![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/1.jpg) | ![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/2.jpg) | ![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/3.jpg)

Screenshot | Screenshot | Screenshot
------------ | ------------- | -------------
![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/4.jpg) | ![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/5.jpg) | ![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/6.jpg)

# 2) Buttons

Screenshot | Screenshot | Screenshot
------------ | ------------- | -------------
![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/b1.jpg) | ![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/b2.jpg) | ![](https://raw.githubusercontent.com/techvootsolutions/TV_Flutter_Component/main/Images/b3.jpg)

# How to use

```
import 'package:flutter/material.dart';
import 'package:flutter_components/flutter_component.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Buttons',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: const Buttons(),
    );
  }
}

class Buttons extends StatefulWidget {
  @override
  _ButtonsPageState createState() => _ButtonsPageState();
}

class _ButtonsPageState extends State<Buttons> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Container(
        width: double.infinity,
        padding: const EdgeInsets.symmetric(horizontal: 20, vertical: 20),
        child: SingleChildScrollView(
          child: Column(
            children: [
  ```
 # Simple Buttons
 ```
              customContainer(
                  child: SuccessButton(
                title: "Success Button",
                onPressed: () {},
              )),

 ```
# Icon Button
 ```
              customContainer(
                child: ButttonWithIcon(
                  icon: Icons.local_cafe,
                  title: "Icon Button",
                  color: Colors.white,
                  buttonColor: Colors.cyan,
                  onPressed: () {},
                ),
              ),
 ```
# Floating Button
 ```
              Wrap(
                children: [
                  FloatingIconButton(
                    icon: Icons.home,
                    onPressed: () {},
                    buttonColor: Colors.orange,
                  ),
                  FloatingIconButton(
                    icon: Icons.home,
                    onPressed: () {},
                    buttonColor: Colors.cyan,
                    color: Colors.white,
                  )
                ],
              ),
 ```
# Line Button
 ```
              customContainer(
                  child: PrimaryLineButton(
                onPressed: () {},
                title: "Line Button",
              )),
              customContainer(
                  child: InfoLineButton(
                textColor: Colors.black,
                onPressed: () {},
                title: "Info Line Button",
              )),
   ```
# Rounded Button
 ```
              customContainer(
                  child: RoundedButtonWithIcon(
                onPressed: () {},
                icon: Icons.title,
                title: "Rounded Button With Icon",
                buttonColor: Colors.green,
              )),
   ```
# Social Button
 ```
              Wrap(
                children: <Widget>[
                  FacebookButton(
                    onPressed: () {},
                  ),
                  TwitterButton(
                    onPressed: () {},
                  ),
                ],
              ),
              SignInWithEmail(
                onPressed: () {},
              ),
              SignInWithGoogle(
                onPressed: () {},
              ),
              SignInWithMicrosoft(
                onPressed: () {},
              ),
              SignInWithApple(
                onPressed: () {},
              ),
             )),
   ```
# Gradiant Button
 ```
              customContainer(
                  child: GradientButton(
                onPressed: () {},
                splashColor: Colors.orange,
                colors: const [
                  Colors.red,
                  Colors.orange,
                ],
                title: "Gradient Button",
              )),
            ],
          ),
        ),
      ),
    );
  }
}

``` 
## Main Contributors

<table>
  <tr>
    <td align="center"><a href="https://github.com/tvPrincy"><img src="https://avatars.githubusercontent.com/u/81419917" width="100px;" alt=""/><br /><sub><b>Varsani Princy</b></sub></a></td>
    <td align="center"><a href="https://github.com/techkevin"><img src="https://avatars.githubusercontent.com/u/37235824" width="100px;" alt=""/><br /><sub><b>Baldha Kevin</b></sub></a></td>
  </tr>
</table>

