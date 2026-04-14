# Android OTP Code Application

## 🚀 Author
Bojan Brankovic 

## Project Overview
This project is an Android OTP (One-Time Password) Verification Application designed to simulate secure user authentication using phone number verification.

The application demonstrates how OTP-based authentication works, where users receive a one-time verification code via SMS and enter it to confirm their identity.

OTP authentication is widely used in modern applications as an additional security layer, ensuring that only the rightful user can access the system. :contentReference[oaicite:0]{index=0}

## Features
- Phone number input and validation  
- OTP generation and sending (SMS-based)  
- OTP verification screen  
- Automatic or manual OTP input  
- Error handling (invalid/expired OTP)  
- Resend OTP functionality  
- Basic session handling after verification  

## Tech Stack
- Java / Kotlin (Android)
- Android SDK
- Firebase Authentication (Phone Auth) / Backend API
- Android Studio

## Application Flow
1. User opens the app  
2. Enters phone number  
3. OTP is sent via SMS  
4. User enters received OTP  
5. System verifies OTP  
6. On success → user is authenticated  
7. On failure → error message displayed  

## Scope of Testing
- OTP sending and delivery  
- OTP validation (correct/incorrect code)  
- Expired OTP handling  
- Resend OTP functionality  
- Network dependency scenarios  
- Session behavior after login  

## Tools Used
- Manual Testing  
- Android Emulator / Real Device (physical device recommended for SMS)  
- Logcat (debugging)  

## Testing Types
- Functional Testing  
- Security Testing (basic)  
- Negative Testing  
- Exploratory Testing  
- Regression Testing  

## Deliverables
- Test Cases  
- Bug Reports  
- Test Execution Report  

## Key Issues Identified
- OTP not received under certain network conditions  
- OTP verification fails despite correct code  
- Delay in OTP delivery  
- Resend OTP button not triggering new code  
- App allows multiple OTP requests without restriction  
- Session starts even with failed verification  

## Important Notes
- OTP testing requires a real device with active SIM card (emulators may not support SMS delivery) :contentReference[oaicite:1]{index=1}  
- Network connectivity is required for OTP request and verification  
- Security depends on proper OTP generation and validation logic  

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/devbojan/android-otp-code-app.git
