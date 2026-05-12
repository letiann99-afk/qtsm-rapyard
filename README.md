# qtsm-rapyard✅ RAP YARD — FULL TRANSFER PACKAGE
This is the complete, ready‑to‑import blueprint.

🧩 1. Project Summary
Rap Yard is a mobile app for recording, uploading, sharing, and listening to rap tracks.
Core features include:

User accounts

Audio recording & upload

Track feed

Likes & listens

Profiles

Analytics events

Clean industrial QTSM branding

If you want a deeper summary:
Project summary

🗄️ 2. Database Schema (Collections)
Users
id

email

passwordHash

handle

avatarUrl

createdAt

Tracks
id

userId

title

description

audioUrl

createdAt

Likes
id

userId

trackId

createdAt

Listens
id

userId

trackId

createdAt

Events
id

userId

type

metadata

createdAt

If you want this in SQL or JSON format:
Backend schema

🔌 3. API Specification
Auth
POST /auth/register

POST /auth/login

Tracks
GET /tracks

GET /tracks/:id

POST /tracks

POST /tracks/:id/like

POST /tracks/:id/listen

Upload
POST /tracks/upload

Analytics
POST /events

📱 4. Frontend Structure (Adalo‑Ready)
Screens
Login

Register

Feed

Create Track

Profile

Settings (optional)

Components
Button

Card

Typography

Icon set (mic, bolt, wrench, fence)

Audio player

Audio recorder

Navigation
Auth Stack → Main Tabs

Tabs: Feed | Create | Profile

If you want the full screen‑by‑screen build:
Frontend structure

🎨 5. Branding & Logo
Your QTSM industrial logo is already generated.
Brand identity:

Industrial metallic tones

Matte black

Orange/yellow energy accents

Strong geometric shapes

Mic + city + waveform motif

If you want a full brand kit:
Brand assets

🔧 6. Adalo Integration Guide
Step 1 — Create Collections
Create collections matching the schema above:

Users

Tracks

Likes

Listens

Events

Step 2 — Add Custom Actions
For each API endpoint, create a Custom Action in Adalo:

Login

Register

Upload audio

Create track

Like track

Log listen

Log events

Step 3 — Build Screens
Connect Login/Register to Auth actions

Feed screen → List of Tracks collection

Create screen → File picker + Custom Action upload

Profile screen → Filter Tracks by Logged‑In User

Step 4 — Add Audio Components
Use Adalo’s audio player

Use file picker for uploads

Step 5 — Add Analytics
Trigger events on:

Login

Track upload

Play

Like
