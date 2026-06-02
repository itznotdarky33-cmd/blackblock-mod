# 🔨 Termux se Black Block Mod Build Karne ki Guide

## Step 1 — Termux Install Karo
- F-Droid se Termux download karo (Play Store wala outdated hai)
- Link: https://f-droid.org/packages/com.termux/

## Step 2 — Termux mein yeh commands chalaao (ek ek karke)

```bash
pkg update && pkg upgrade -y
pkg install wget unzip git -y
```

## Step 3 — Java 8 Install Karo
```bash
pkg install openjdk-17 -y
java -version
```

## Step 4 — Gradle Install Karo
```bash
cd ~
wget https://services.gradle.org/distributions/gradle-7.3-bin.zip
unzip gradle-7.3-bin.zip
export PATH=$PATH:~/gradle-7.3/bin
gradle -v
```

## Step 5 — Mod Project Copy Karo
- Apne phone ki Files app se `blackblock-mod` folder ko
  `/sdcard/blackblock-mod/` mein rakho
- Phir Termux mein:
```bash
cp -r /sdcard/blackblock-mod ~/blackblock-mod
cd ~/blackblock-mod
```

## Step 6 — Build Karo!
```bash
chmod +x gradlew
./gradlew build
```
⚠️ Pehli baar bohot time lagega (Minecraft download hoga ~1-2GB)
Internet strong hona chahiye!

## Step 7 — JAR File Nikalo
```bash
ls build/libs/
```
`blackblock-1.0.0.jar` milegi!

## Step 8 — Mojo Launcher mein Install Karo
```bash
cp build/libs/blackblock-1.0.0.jar /sdcard/
```
- Mojo Launcher > mods folder mein daalo
- Forge 1.16.5 se launch karo
- Creative inventory > Building Blocks mein **Black Block** milega! ✅

---
## ❓ Problem aaye toh mujhe bata dena, fix kar dunga!
