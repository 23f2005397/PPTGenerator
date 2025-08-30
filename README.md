# PPTGenerator
Auto-Generate a Presentation
**Features**

* 📝 **Input Options**: Paste large chunks of text, markdown, or prose.
* 🎯 **Guidance**: Add a one-line instruction for tone or structure (e.g., “make it an investor pitch deck”).
* 🔑 **Bring Your Own API Key**: Supports OpenAI, Anthropic, Gemini, and more (keys are never stored or logged).
* 🎨 **Template Reuse**: Upload your `.pptx` or `.potx` template to apply colors, fonts, and layouts.
* 🖼️ **Image Reuse**: Recycles existing images from your uploaded template.
* 📥 **Instant Download**: Outputs a new `.pptx` file you can download directly.
* ⚡ **Smart Splitting**: Automatically divides your text into a reasonable number of slides.
* 🔒 **Privacy First**: No logging or saving of user text, keys, or files.

* ## 🛠️ Architecture

* **Frontend**:

  * Responsive HTML + Tailwind UI
  * Handles text input, template upload, and file download
  * Provides toasts, progress feedback, and history of past generations

* **Backend (FastAPI)**:

  * Accepts text, guidance, API key, and template
  * Splits input intelligently into slide sections
  * Maps new content onto the uploaded template’s style, layout, fonts, and images
  * Generates `.pptx` output using `python-pptx`

---

## 🌟 Optional Enhancements

* Auto-generate speaker notes
* Offer prebuilt guidance templates (*sales deck, investor pitch, research summary*)
* Add live slide previews before download
* Retry logic + better error handling for unstable APIs

---

## 📄 License

MIT License – free to use, modify, and share.
