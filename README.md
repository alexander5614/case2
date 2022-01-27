# import 'package:flutter/material.dart';

  void main() {
    runApp(const MyApp());
  }

  class MyApp extends StatelessWidget {
    const MyApp({Key? key}) : super(key: key);

    // This widget is the root of your application.
    @override
    Widget build(BuildContext context) {
      const borderStyle = OutlineInputBorder(
        borderRadius: BorderRadius.all(Radius.circular(36)) ,
        borderSide: BorderSide(
          color: const Color(0xFFeceff1), width: 2));
      const linkTextStyle = TextStyle(
        fontSize: 18,
        fontWeight: FontWeight.bold ,
        color: Color(0xFF0079D0),
      );
      return MaterialApp(
        home: Scaffold(
            body: Container(
              decoration: const BoxDecoration(
                                       image: DecorationImage(
                                           image: AssetImage("),
                fit: BoxFit.cover,)
              ),
              width: double.infinity,
              height: double.infinity,
              padding: EdgeInsets.symmetric(horizontal: 50 ),

              child: SingleChildScrollView(
                child: Column(children: [
                  SizedBox(height: 150,),
                  const SizedBox(width: 110,height: 84,child: Placeholder() ,),
                  SizedBox(height: 20,),
                  Text('Введите логин в виде 10 цифр номера телефона',
                    style: TextStyle(fontSize: 16, color: Color.fromRGBO(0,0,0,0.6)),),
                  SizedBox(height: 20),
                  SizedBox(width: 224,
                    child: TextField(
                      keyboardType: TextInputType.phone,
                        decoration: InputDecoration(
                            filled: true,
                            fillColor: Color(0xFFeceff1),
                            enabledBorder: borderStyle ,
                            focusedBorder: borderStyle,
                            labelText: 'Телефон',
                         ),
                    ),
                  ),
                  SizedBox(height: 20,),
                  const SizedBox(width: 224,
                    child: TextField(
                      obscureText: true,
                        decoration: InputDecoration(
                        filled: true,
                        fillColor: Color(0xFFeceff1),
                        enabledBorder: borderStyle ,
                        focusedBorder: borderStyle,
                        labelText: 'Пароль',
                        ),
                     ),
                    ),
                  SizedBox(height: 28,),
                  SizedBox(width: 154, height: 42, child:
                   ElevatedButton(onPressed: () {},
                   child: Text('Войти'),
                   style: ElevatedButton.styleFrom(
                     primary: Color(0xFF0079D0),
                     shape: RoundedRectangleBorder(
                      borderRadius: BorderRadius.circular(36.0),
      ),
      ),
      )
      ),
                  SizedBox(height: 62,),
                  InkWell(child: Text('Регистрация', style: linkTextStyle
  ,
                   ), onTap: () {},),
                  SizedBox(height: 20,),
                  InkWell(child: Text('Забыли пароль?', style: linkTextStyle
  ,
      ),
            onTap: () {}),
                ],),
              ),
            ),
        ),
          // This is the theme of your application.
          //
          // Try running your application with "flutter run". You'll see the
          // application has a blue toolbar. Then, without quitting the app, try
          // changing the primarySwatch below to Colors.green and then invoke
          // "hot reload" (press "r" in the console where you ran "flutter run",
          // or simply save your changes to "hot reload" in a Flutter IDE).
          // Notice that the counter didn't reset back to zero; the application
          // is not restarted.
               );
    }
  }

case2

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
