# capacitor-walkthrough

## Start Ionic Project

สร้าง ionic project ตามปกติ แต่ให้ตอบ N ตอนที่ถามเรื่อง cordova

```bash
ionic start <APP NAME> tabs
cd <APP NAME>
```

## Build your Ionic App

รันคำสั่งเตรียมไฟล์ application ไว้ในโฟลเดอร์ www

```bash
npm run build
```

## Install Capacitor

```bash
npm install --save @capacitor/cli @capacitor/core
```
## Remove Cordova Splash

```bash
npm uninstall --save cordova-plugin-splashscreen
```

## สร้าง config ของ Capacitor

```bash
npx cap init
```

## Add Platforms
```bash
npx cap add ios
npx cap add android
npx cap add electron
```

## คำสั่งเปิดโปรแกรมที่ใช้ในการ build ของแต่ละ platform

```bash
npx cap open ios
npx cap open android
```

## คำสั่งรัน electron

```bash
cd electron
npm run electron:start
```

## Sync โค้ดแอพไปที่ Capacitor

```bash
npm run build
npx cap copy
```
