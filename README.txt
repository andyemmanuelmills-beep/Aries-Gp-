Aries AI - Debug-ready Android Studio Project (with Tutorial)

What is included:
- Aries-themed UI with tutorial screen
- CameraX preview stub and enrollment buttons
- Deferred BLE pairing manager that waits for battery >= threshold
- CloudBrain placeholder for online AI responses (configure API key)
- Offline fallback message and basic helper modules
- User assets preloaded: user_photo.jpg, user_voice.m4a, aries_logo_clean.png
- Placeholder TFLite model files under app/src/main/assets/models/ (replace with real models)
- GitHub Actions workflow (.github/workflows/android-build.yml) that builds a debug APK artifact

How to build (GitHub Actions):
1. Create a GitHub repo and push the project contents (do not upload ZIP directly).
2. On push to main, the Actions workflow will run and produce an artifact named AriesAI-debug-apk.
3. Download the APK artifact to your phone and install.

Important:
- Replace the placeholder TFLite models with working MobileFaceNet and speaker embedding TFLite files.
- Edit app/src/main/java/com/ariesgp/starter/ai/CloudBrain.kt and set your API endpoint and key for online responses.
- Update pairing target in MainActivity if desired (targetNameOrAddress).
