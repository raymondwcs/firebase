# Google Firebase Hosting - A Quick Tutorial

## Introduction
This tutorial outlines the steps of deploying a simple Web app to Google Firebase

## Part 1
1. Check out an *incomplete* Web app that computes simple interest.
```
git clone https://github.com/raymondwcs/firebase
```
2. Open `public\index.html` in your Web browser

The **CALCULATE** button isn't working yet.  Let's fix this!

## Part 2
3. Insert the following into the `handleSubmit(event)` function.
```
var i = this.state.principal * this.state.rate * this.state.time;
this.setState({interest:i});
```
4. Reload `public/index.html`. The **CALCULATE** button should be working now!

## Part 3
5. Create a Google Firebase Project at the following URL.  Write down the **Project-ID**
```
https://console.firebase.google.com
```
6. Deploy your Web app to Google Firebase
```
cd ~/firebase
firebase login
firebase use Project-ID
firebase deploy
```
7. Goto https://**Project-ID**.firebaseapp.com
