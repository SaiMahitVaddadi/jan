# Routing Jan through the local LiteLLM gateway

Jan is a desktop app — model providers are configured in the Settings UI
at runtime, not via a repo env file.

To route Jan through the gateway:

1. Launch Jan.
2. Settings → **Model Providers** → choose **OpenAI** (or any
   OpenAI-compatible entry; "OpenAI Compatible" if your version exposes
   it).
3. Set:
   - **API Key:** `sk-litemagic-123`
   - **API Endpoint / Base URL:** `http://localhost:4000/v1`
4. Refresh models. Models exposed by the LiteLLM config become available
   in Jan's model picker.

Jan also ships its own local engine (Cortex). The above only affects
remote / OpenAI-style providers — local Cortex models stay local.
