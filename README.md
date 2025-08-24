📖 Daily Quran Poster Generator (n8n + Gemini Workflow)

This project is a no-code automation built in n8n
 that automatically generates daily Quran verse posters and saves them to Google Drive.

🚀 Features

AI-driven Verse Selection: Uses Google Gemini to fetch Quranic verses in sequence with authentic references (chapter, verse number, Arabic text, translation).

Authentic Content: Ensures accuracy by directing Gemini to reference existing Quran text available on the web.

Poster Generation: Converts verse + translation into a styled poster image using HTML→Image API (HCTI).

Google Drive Upload: Saves each poster into Google Drive with proper filenames (SurahName • VerseNumber.jpg).

Flexible Scheduling: Triggered with n8n’s schedule node (e.g., daily or every 5 minutes for testing).

🔧 Workflow Overview

Schedule Trigger → defines the posting interval.

Gemini Node → fetches the next Quran verse (Arabic + translation) with correct reference.

Formatting Node → cleans Gemini output into structured JSON.

Prepare Poster Text → escapes text safely for HTML.

Build Poster → creates a poster image using HTML & CSS styling.

Download Poster → retrieves the generated image as binary.

Google Drive Upload → saves the poster file in Drive.

📂 Output

Posters saved automatically to Google Drive.

File names: SurahName • VerseNumber.jpg

Example: Al-Baqarah • 2:255.jpg

⚙️ Requirements

n8n (self-hosted or cloud).

Google Gemini API key.

HCTI API key (for HTML→Image conversion).

Google Drive credentials (for upload).

🌟 Use Cases

Daily Quran poster reminders.

Auto-generated study materials.

Content pipeline for social media (Instagram, Twitter, etc. — can be added later).
