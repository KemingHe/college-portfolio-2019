---
layout: post
title:  "Sixth Sense Project - Ongoing"
date:   2019-12-01 12:00:00 -0400
categories: projects
---

<style type="text/css">
.image-right {
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}

.image-left {
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: left;
}

img.shrinked{
	height: 90%;
	width: 90%;
}
</style>

### Overview

The [Sixth Sense Project]( https://github.com/Tickloop/6ixthSense) aims to help the visually impaired to better navigate the world with computer vision technologies. The project is designed by [Keming]( https://github.com/KemingHe), [Pulkit]( https://github.com/Tickloop), and [Karthik]( https://github.com/karthikp32), and has been in development since early 2019. Project Sixth Sense consists of three parts: 
1. The user would stream video to the Amazon Web Service (AWS), through a smartphone app; 
2. The AWS [Rekognition]( https://aws.amazon.com/rekognition/) will analyze the video and return a list of street objects to the smartphone;
3. The smartphone app would warn the user of incoming obstacles by sending vibration signals to two wristbands, one on each arm. 

### Responsibility

My responsibility is to develop a prototype of the smartphone app that successfully uploads videos/images to AWS, and then call the Rekognition API to analyze the upload in real-time. From October to December of 2019, I have been working with Android Studio and the AWS Software Development Kit to bring this project to life. I created a roadmap for the team, and documented my development through progress reports.

<p align="center">
  <img class="shrinked" src="../../../../assets/images/6thSenseProjectRoadmap.png" alt="Roadmap">
  <br>
  Figure 1 Roadmap of Sixth Sense Project, AU19 Semester
  <br>
  <br>
  List of my progress reports:
  <br>
  <a href="../../../../assets/pdfs/6thSense_Android_Keming_ProgressReport_1_ver10.27.19.pdf">Android Dev - Progress Report 1 (10/20-10/26)</a>
  <br>
  <a href="../../../../assets/pdfs/6thSense_Android_Keming_ProgressReport_2_ver11.03.19.pdf">Android Dev - Progress Report 2 (10/27-11/02)</a>
  <br>
  <a href="../../../../assets/pdfs/6thSense_Android_Keming_ProgressReport_3_ver11.17.19.pdf">Android Dev - Progress Report 3 (11/11-11/17)</a>
  <br>
  <a href="../../../../assets/pdfs/6thSense_Android_Keming_ProgressReport_4_ver12.01.19.pdf">Android Dev - Progress Report 4 (11/18-12/01)</a>
  <br>
  (More to be updated...)
</p>

### Forward

The Sixth Sense Project is currently still in its prototyping phase. The team and I have taken much inspiration from existing projects and open-sourced softwares, listed in the reference section below. Our next step is to finish the Minimal Viable Product, and start conducting research on the effectiveness of our creation.


### Reference

Android. (2019, November 29). android/camera-samples. Retrieved from [https://github.com/android/camera-samples](https://github.com/android/camera-samples).

Awslabs. (2019, November 18). awslabs/aws-sdk-android-samples. Retrieved from [https://github.com/awslabs/aws-sdk-android-samples/tree/master/S3TransferUtilitySample](https://github.com/awslabs/aws-sdk-android-samples/tree/master/S3TransferUtilitySample).

SA, A. (2019, April 26). AWS Rekognition in Android. Retrieved from [https://medium.com/how-to-integrate-aws-rekognition-in-android/aws-rekognition-in-android-9d16f16d591c](https://medium.com/how-to-integrate-aws-rekognition-in-android/aws-rekognition-in-android-9d16f16d591c).
