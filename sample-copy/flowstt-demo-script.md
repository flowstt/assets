# FlowSTT Demo Script -- TTS Sample Copy

Sample copy for text-to-speech synthesis. Use these passages to test and
demonstrate FlowSTT transcription. Each section is self-contained and varies in
length, complexity, and vocabulary to exercise different aspects of the
transcription engine.

---

## 1. Introduction (Short)

FlowSTT is a free, privacy-first speech-to-text application that runs entirely
on your computer. Your voice never leaves your machine. There are no
subscriptions, no cloud services, and no sign-ups required. Just download, set
up, and start talking.

---

## 2. How It Works (Medium)

FlowSTT uses OpenAI's Whisper model to transcribe your speech locally. When you
speak, the app captures audio from your microphone, detects when you start and
stop talking, and sends each phrase to the Whisper engine running right on your
hardware. If you have a compatible graphics card, FlowSTT will use GPU
acceleration to transcribe faster. Otherwise, it falls back to your CPU
automatically. The transcribed text is copied to your clipboard and, optionally,
pasted directly into whatever application you're working in.

---

## 3. Privacy and Security (Short)

Privacy is not just a feature of FlowSTT. It is the foundation. Every bit of
audio processing happens on your local machine. Your recordings are never
uploaded, never stored on a remote server, and never used to train a model. When
you close the app, the audio is gone. Your words belong to you.

---

## 4. Transcription Modes (Medium)

FlowSTT offers two ways to capture your speech. In automatic mode, the app
listens continuously and uses voice activity detection to figure out when you're
speaking. It analyzes multiple audio features, including amplitude, zero-crossing
rate, and spectral centroid, to distinguish your voice from background noise like
keyboard clicks or mouse sounds. When you stop talking, the phrase is
transcribed.

In push-to-talk mode, you hold down a hotkey to record, and release it to
transcribe. This gives you precise control over exactly what gets captured. You
can configure any key or key combination as your hotkey, and you can switch
between modes instantly with a separate toggle key.

---

## 5. Audio Visualization (Short)

FlowSTT includes a real-time audio visualization window. It displays a scrolling
waveform, a spectrogram, and a detailed speech activity graph. You can see
exactly when the app detects your voice, where word boundaries fall, and how
your speech energy changes over time. It is a great tool for understanding how
the speech detection works and for tuning your microphone setup.

---

## 6. System Audio and Echo Cancellation (Medium)

Beyond microphone input, FlowSTT can capture system audio, which is the sound
playing through your speakers or headphones. This is useful for transcribing
meetings, podcasts, or any audio from other applications. You can also use mixed
mode, which combines your microphone and system audio into a single stream. In
mixed mode, FlowSTT applies WebRTC echo cancellation to separate your voice from
the system audio, so your own speech is captured cleanly without picking up
whatever is playing in the background.

---

## 7. The Command Line Interface (Medium)

FlowSTT comes with a full command-line interface for users who prefer working in
a terminal. The CLI lets you list audio devices, start and stop transcription,
manage Whisper models, check GPU status, and configure every setting, all without
opening the graphical interface. Output can be formatted as JSON for scripting
and automation. If the FlowSTT app is not already running, the CLI will launch it
in headless mode automatically, so you can use FlowSTT entirely from the command
line if you choose.

---

## 8. Cross-Platform Support (Short)

FlowSTT runs on Windows, macOS, and Linux. On Windows, it uses WASAPI for audio
and includes CUDA support out of the box. On macOS, it uses CoreAudio and Metal
GPU acceleration. On Linux, it supports PipeWire and PulseAudio. The app adapts
to your operating system automatically so you get the best performance on
whatever platform you use.

---

## 9. Setup and First Run (Medium)

When you first launch FlowSTT, a setup wizard walks you through everything you
need. It downloads the Whisper speech model, which is about one hundred and
forty-five megabytes, and stores it locally. Then it helps you select your
microphone and shows a live audio level meter so you can verify it is working.
You pick your preferred transcription mode, and finally, you do a quick live test
to make sure everything is connected. The whole process takes just a couple of
minutes.

---

## 10. Transcription History (Short)

Every phrase FlowSTT transcribes is saved to a local history file with a
timestamp. You can scroll through your recent transcriptions, copy any entry to
the clipboard, or delete entries you no longer need. Audio recordings are cached
temporarily so you can play them back, but they are automatically cleaned up
after twenty-four hours while your text history is kept.

---

## 11. Full Feature Overview (Long)

FlowSTT is a desktop speech-to-text application built for people who care about
privacy and want reliable transcription without depending on an internet
connection. It is completely free, with no subscriptions, no accounts, and no
data collection.

At its core, FlowSTT runs the Whisper speech recognition model locally on your
machine. It supports GPU acceleration through CUDA on Windows, Metal on macOS,
and optionally CUDA on Linux, with automatic fallback to CPU processing when a
compatible graphics card is not available.

The app captures audio from three types of sources: your microphone, your system
audio output, or a mix of both. When using mixed mode, WebRTC acoustic echo
cancellation separates your voice from the system audio so transcription stays
clean.

FlowSTT's automatic speech detection is more than a simple volume threshold. It
performs multi-feature analysis on the audio stream, examining amplitude,
zero-crossing rate, and spectral centroid to identify voiced speech, whispered
speech, and transient sounds like keyboard and mouse clicks. A lookback buffer
captures the true onset of each phrase, and word boundary detection ensures that
segments are split at natural pauses rather than mid-word.

For users who want manual control, push-to-talk mode lets you record only while
holding a configurable hotkey. You can assign any key or combination, set up
multiple bindings, and switch between automatic and push-to-talk modes instantly
with a dedicated toggle hotkey.

Transcribed text is automatically copied to the clipboard and can be pasted into
the active application with a simulated keystroke. The paste behavior is
configurable, and FlowSTT is smart enough to suppress it when its own window is
in the foreground.

A real-time visualization window shows a scrolling waveform, an FFT-based
spectrogram with a heat-map color gradient, and a multi-layer speech activity
graph. The speech activity view plots amplitude, zero-crossing rate, and spectral
centroid as separate lines, with markers for speech onsets, transient sounds, and
word breaks.

FlowSTT includes a full command-line interface with commands for device
management, transcription control, model management, GPU status, and
configuration. The CLI supports JSON output for scripting, quiet and verbose
modes, and will auto-launch the app in headless mode if it is not already
running.

The application supports light, dark, and auto themes. It integrates with the
system tray for unobtrusive background operation. And a first-run setup wizard
handles model download, device selection, and a live transcription test so you
can be up and running in minutes.

FlowSTT is currently in public beta for Windows and macOS, with Linux support
in development.
