
Project: VoiceGPT Telegram Bot
Overview
VoiceGPT Telegram Bot is an intelligent assistant that runs inside Telegram. It can understand both text and voice messages, generate smart replies using OpenAI's GPT model, and even speak back to you. When you send a voice message, the bot transcribes it with Whisper, processes it with GPT, converts the answer to speech using OpenAI's TTS, and sends the voice reply back to you – all automatically.

Key Features
Dual‑mode interaction – Works with text and voice messages.

Speech‑to‑text – Uses OpenAI Whisper to accurately transcribe voice notes.

AI reasoning – Powered by GPT‑4o‑mini (or GPT‑3.5‑Turbo) for intelligent, human‑like answers.

Text‑to‑speech – Converts the AI's text reply into natural‑sounding speech with OpenAI TTS.

Seamless voice handling – Automatically converts audio formats (OGG ↔ MP3) so that Telegram and OpenAI APIs can talk to each other.

Production‑ready – Includes error handling, logging, and automatic cleanup of temporary files.

How It Works (Step by Step)
You send a voice message (or text) to the bot on Telegram.

The bot downloads the voice file (OGG format) and converts it to MP3.

Whisper transcribes the MP3 into text.

The transcribed text is sent to GPT, which generates a reply.

The bot converts that reply into speech using OpenAI's TTS (MP3 output).

The MP3 is converted back to OGG (the format Telegram expects for voice messages).

The bot sends the voice message back to you, and you can listen to the AI's spoken answer.

For text messages, the bot simply replies with text – no conversion steps needed.

Technologies Used
Python 3.8+ – Core language.

python‑telegram‑bot – Telegram API wrapper.

OpenAI API – Whisper (speech‑to‑text), GPT (reasoning), TTS (text‑to‑speech).

pydub + FFmpeg – Audio format conversion.

python‑dotenv – Environment variable management.

Why This Bot Is Useful
Hands‑free interaction – just talk, no typing.

Great for learning languages, getting quick answers, or simply having a conversation.

Fully private – you control your own API keys and the bot runs on your own server.

Easily extensible – you can add conversation memory, change voices, or switch to a different AI model.

Example Use Cases
Voice assistant – Ask questions while cooking, driving, or walking.

Language practice – Speak in a foreign language, get corrections or translations.

Accessibility – Helps users who find typing difficult.

Fun & entertainment – Have a spoken conversation with an AI.
