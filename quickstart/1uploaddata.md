# 1 Upload Data

## Quick Start

## 1 Add a new device

For getting started on DeviceBit platform, the first step is to add a new device. Log into the IOT platform \(If you don’t have the account you need to sign up first\). Sign up a DeviceBit Account \([www.devicebit.com](https://github.com/Luyufei1983/DeviceBit/tree/af21180bdb310cbff790aebd866c3dfed3218fd5/www.devicebit.com)\) ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-1.jpg) Pic.1 Sign Up As shown in Pic2, go to _**My Devices -&gt; Devices -&gt; Add A device**_, fill in the information and then save. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-2.jpg)

Pic.2 Create a new device

## 2 Add sensors & controllers

The next step is to add a new sensor or controller connected to your device.

### 2.1 Add a new sensor

As shown in Pic3, go to _**My Devices -&gt; Sensors&Controllers -&gt;Sensors,**_ and then click on _**Add**_ button to create a new sensor. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-3.jpg) Pic.1 Add a new sensor !\[\]\[4\]

## 3 Data Upload Simulation

This tutorial mainly introduces how to simulate data upload by using API testing tool. **Hardware** No hardware is required. Only simulate data upload by API testing tool provided by Devicebit platform. **Procedure：** 1 Sign up a DeviceBit Account \([www.devicebit.com](https://github.com/Luyufei1983/DeviceBit/tree/af21180bdb310cbff790aebd866c3dfed3218fd5/www.devicebit.com)\) ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-1.jpg)

Pic.1 Sign Up

### 3.1 Add My Device, Sensors: Humidity and Temperature

\(The steps are as follows. Note: note down the ID, for it will be used in Api calling.\)

### 3.2 Add A Device

After login, go to My Devices -&gt; Devices-&gt;Add a Device First, click on Devices -&gt; Add A Device , as the picture1 below. After entering the related information, click on Save. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-2.jpg)

### 3.3 Add Humidity

The next step is to add the humidity sensor. Go to**My Devices-&gt; Sensors&Controllers-&gt;Sensor**, click on **Add**.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-3.jpg) Pic.3 Sensors Then there will be the _**Add A Sensor**_ page. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-7.jpg) Pic.4 Add Humidity

### 3.3 Add Temperature

Add the _**Temperature**_ sensor in the same way. Please see the following picture. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-8.jpg) Pic.5 Add Temperature After setting up, as picture 5 shows, note down the _**ID**_ because it will be used in Api calling. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-9.jpg)

Pic.6 Sensor ID

### 3.4 Data Simulation

Now, let's move on to simulate data upload by using Api testing tool. At the home page \(the website is www.devicebit.com\) click on _**Documentation**_

Pic.7 Home Page and then go to **API Directory-&gt; Sensor -&gt;Upload Sensor Data** ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-10.jpg) Pic.8 API Directory Website [https://www.devicebit.com/dev/apitest/203](https://www.devicebit.com/dev/apitest/203)

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-11.jpg) Pic.9 On-line test Click on _**on-line test**_ ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-12.jpg) Pic.10 API Testing Tool Enter your **Userkey** Enter _**Device ID**_ at API URL [http://www.devicebit.com/api/V1/gateway/UpdateSensors/{device](http://www.devicebit.com/api/V1/gateway/UpdateSensors/{device) ID} [（01 for exampe）](http://www.lewei50.com/api/V1/gateway/UpdateSensors/你的网关号) After entering the device ID, the APIURL is: [http://www.devicebit.com/api/V1/gateway/UpdateSensors/01](http://www.devicebit.com/api/V1/gateway/UpdateSensors/01) ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-13.jpg) Pic.11 Userkey & Device No. Change _**T1**_ to _**Temperature**_ for _**Name**_; change _**1**_ to _**32**_ for **Value\***; Change _**01H1**_ to _**Humidity**_ for _**Name**_; change _**96.2**_ to _**75**_ for _**Value**_. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-14.jpg) Pic.12 Post Data Click on _**Run**_, and then the request detail will be displayed. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-15.jpg) Pic.13 Request Detail At last, Go to _**My IOT -&gt; Sensors&Controllers-&gt;Sensor List**_, you will see the following value. !\[\]\[16\] Pic.14 The Value Well Done! Your data upload is successfully simulated by using API testing tool!

The following part will introduce how to set Notice Groups, and receive email alerts

## 4 Alert

The following part will introduce how to set Notice Groups, and receive email alerts.

## 4.1 Add A New Contact

Click on Notice Groups -&gt; Contacts -&gt; New Contact ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-17.jpg)

Enter the name, Email etc. of this contact and then click on Save. ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-18.jpg)

Add more contacts in the same way.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-19.jpg)

## 4.2 Add A New Group

Go to Notice Groups -&gt; Add Group

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-20.jpg)

Enter the group name, tick the contacts, and save.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-21.jpg)

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-22.jpg)

## 4.3 Alarm Settings

Go to List, and click on Edit.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-23.jpg) ![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-24.jpg)

Set the normal temperature range for your device and select the notice group, e.g. the Temperature group which is just set. Then, set the normal humidity range in the same way.

Then, click on Save and the settings are successfully saved. Please remember the ID of the sensors \(H1, T1\), for they will be used in the following calling step.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-25.jpg)

After settings, simulate data upload as the last chapter mentioned.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-26.jpg)

Meanwhile, you will receive the following alarms by Email.

![](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-27.jpg)

\[16\]: [https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-16.jpg](https://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/devicebitmanual-xj-20180930-16.jpg)

