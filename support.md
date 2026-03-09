# BonzAI Support

Welcome to BonzAI support page. Here you'll find answers to common questions and resources to help you get started.

## About BonzAI

BonzAI (BonzAI-online) is a privacy-first AI assistant that runs directly on your iPhone, iPad, or Mac. Chat with powerful AI models locally on your device or connect to external AI services.

## Getting Started

1. **Download BonzAI** from the App Store
2. **Choose your AI model:**
   - Use Apple Intelligence (built-in on compatible devices)
   - Download local models for offline use
   - Connect to external APIs (OpenAI, Gemini, Mistral, etc.)
3. **Start chatting** with your AI assistant

## Key Features

- 🤖 **Multiple AI Providers**: Apple Intelligence, local models (llama.cpp), OpenAI, Google Gemini, Mistral, Anthropic Claude
- 🔒 **Privacy First**: Local inference keeps your data on your device
- 📱 **Cross-Platform**: Works on iPhone, iPad, and Mac
- 🎨 **Modern Interface**: Native SwiftUI design
- 🔧 **Customizable**: Adjust temperature, top-p, context length, and more
- 🧰 **Tool Support**: Web search, weather, location, and extensible MCP tools

## Frequently Asked Questions

### How do I add a local AI model?

1. Go to **Settings** → **Available Models**
2. Tap **Add Model**
3. Select a model from the catalog or Enter a HuggingFace GGUF model URL
4. Wait for the download to complete
5. Select the model

### Why does the app request local network access?

BonzAI uses local network access for two purposes:

- **Internal processing**: The llama.cpp inference engine uses a localhost-only HTTP server (127.0.0.1:8080) for AI model processing. This server is not accessible from outside your device.
- **External services** (optional): If you configure external AI services like Ollama or LM Studio running on your local network, the app needs permission to connect to them.

Your data never leaves your device unless you explicitly choose to use external cloud services.

### How do I connect to external AI services?

1. Go to **Settings** → **Available Models**
2. Tap **Add Model**
3. Select your provider (OpenAI, Gemini, etc.)
4. Enter your API key
5. Select the model

### Is my data private?

Yes! BonzAI prioritizes your privacy:

- **Local models**: All processing happens on your device. No data is sent anywhere.
- **External services**: When you use cloud APIs, data is sent only to the provider you selected. BonzAI does not store or collect your conversations.
- **No tracking**: We don't track your usage or collect analytics about your conversations.

See our [Privacy Policy](privacy-policy.html) for complete details.

### Can I use BonzAI offline?

Yes! When using local models (llama.cpp) or Apple Intelligence on compatible devices, BonzAI works completely offline.

### What are the system requirements?

- **iOS/iPadOS**: 26.0 or later
- **macOS**: 26.0 or later
- **Apple Intelligence**: Requires compatible devices (iPhone 15 Pro or later, M1 Mac or later)
- **Local models**: Recommended 4GB+ free storage and 8GB+ RAM

### How do I delete my conversations?

1. Go to **History**
2. Swipe left on a conversation (left click on macOS)
3. Select **Delete**

You can also delete all app data through iOS Settings → BonzAI → Clear Data.

### The app is not responding or crashes. What should I do?

1. **Force quit** the app and restart it
2. **Check storage**: Large models require significant disk space
3. **Update**: Make sure you're running the latest version from the App Store
4. **Report the issue**: Contact support (see below)

## Contact & Support

### Email Support

For technical issues, feature requests, or general questions:
📧 **thomas.leconte.developer@gmail.com**

### Community

Join our community discussions:
💬 [GitHub Discussions](https://github.com/thom-dev-fr/BonzAI-online/discussions)

### Bug Reports

Report bugs or view known issues:
🐛 [GitHub Issues](https://github.com/thom-dev-fr/BonzAI-online/issues)

## Additional Resources

- [Privacy Policy](privacy-policy.html)
- [Terms of Use](terms.html)

---

**Need more help?** Don't hesitate to reach out via email or GitHub Discussions.

© 2025-2026 BonzAI - Thomas LECONTE
