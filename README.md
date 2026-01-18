# LIZA-PAIR-V1

LIZA-AI BOT - WhatsApp Pair Code Generator
Overview
A Node.js Express web application that generates WhatsApp pair codes for linking devices using the WhatsApp Web protocol via @whiskeysockets/baileys library.

Project Structure
index.js - Main Express server entry point
pair.js - Pair code generation route handler
qr.js - QR code generation route handler
pair.html - Frontend UI for the pair code generator
mega.js - Additional module
Tech Stack
Runtime: Node.js 20+
Framework: Express.js
WhatsApp Protocol: @whiskeysockets/baileys
Phone Validation: awesome-phonenumber
QR Code: qrcode, qrcode-terminal
Running the Application
The server runs on port 5000 and is configured to listen on 0.0.0.0 for Replit compatibility.

npm start
Routes
GET / - Main UI (pair.html)
GET /pair?number=<phone> - Generate pair code for phone number
GET /qr - QR code generation endpoint
