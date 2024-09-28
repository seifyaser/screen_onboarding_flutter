# lottie_screen_onboarding_flutter

lottie Intro Screen Onboarding is a flutter plugin that helps you make a fast intro for your app with easier and best ways using lottie files and images you want

## Animation

<p>
<img src = "https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExNTNmajh6aDA2anNvb2hwcmY4Y2M2MzVhMnVyY3YydnpiaHp5dWJpMiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/LQM1MAMU4I7wCbOrkD/giphy.gif" align = "center" height = "550px"/>
<img src = "https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExY3BuaDhncXRlN2J2aXVxdmp6OXV2aTNwMndwbWxtOXNsYTJjaTJudCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/TTHXqedEYWJvGEYfpc/giphy.gif" align = "center" height = "550px"/>
<img src = "https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWxmcG8zNjNuaGkwbjBjNmcyNWFha2k0b3IweDY1NXFtb2RzNGhzaSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/mCQRQV93zTDTQi9VGs/giphy.gif" align = "center" height = "550px"/>
</p>

## Usage


```dart
import 'package:flutter/material.dart';
import 'package:intro_screen_onboarding_flutter/introduction.dart';
import 'package:intro_screen_onboarding_flutter/introscreenonboarding.dart';
import 'package:weather/screens/homepage.dart';

class onBoarding extends StatefulWidget {
  const onBoarding({super.key});

  @override
  State<onBoarding> createState() => _MyWidgetState();
}

class _MyWidgetState extends State<onBoarding> {
  final List<Introduction> list = [
    Introduction(
      lottieUrl: 'assets/Welcome.json',
     title: 'Welcome to WeatherCast',
      subTitle: 'Enjoy effortless daily weather updates and stay ahead of the weather.',
      ),
    Introduction(
      lottieUrl: 'assets/location.json',
     title: 'At Your Location',
      subTitle: 'Know the weather anytime with one click at your location.'
      ),
      Introduction(
      lottieUrl: 'assets/Searchcity.json',
     title: 'Explore world’s weather!',
      subTitle: 'You can search and discover weather forecasts for cities around the globe.'),
  ];
  @override
  Widget build(BuildContext context) {
    return Scaffold(
   body: SafeArea(
     child: IntroScreenOnboarding(
      introductionList: list,
      onTapSkipButton: () => Navigator.push(context, MaterialPageRoute(builder: ((context) => homepage()))),
      backgroudColor:Color.fromARGB(255, 213, 213, 213),
      foregroundColor: Color.fromARGB(255, 112, 86, 208),
      skipTextStyle: const TextStyle(
        color: Color.fromARGB(255, 112, 86, 208),
        fontSize: 18,
    
      ),
     )
   ), 
    );
  }
}



```

## Getting Started

This project is a starting point for a Dart
[package](https://flutter.dev/developing-packages/),
a library module containing code that can be shared easily across
multiple Flutter or Dart projects.

For help getting started with Flutter, view our 
[online documentation](https://flutter.dev/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.
"# screen_onboarding_flutter" 
