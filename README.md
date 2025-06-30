````markdown
# 🔗 LinkedIn Automation with Image Generation

An end-to-end workflow that automatically generates, formats, and posts engaging content to LinkedIn — complete with AI-generated images!

## 🚀 What it Does

This automation pipeline:
- ⏰ **Schedules** content pulls at optimal times
- 📰 **Scrapes** content topics from curated AI/tech RSS feeds
- 🧠 **Selects high-performing topics** using Gemini 2.5
- ✍️ **Generates a LinkedIn-optimized post** using prompt engineering
- 🖼️ **Creates a matching image** via HuggingFace’s `FLUX.1-schnell` model
- 📤 **Posts to LinkedIn** with text + image via LinkedIn API

## 🔧 Tech Stack

- 🧩 **n8n** (low-code automation)
- 🤖 **Google Gemini API** (text generation)
- 🖌️ **HuggingFace FLUX.1** (image generation)
- 🪝 **LinkedIn API** (posting)

## 📌 Features

- Auto-curated viral topics from multiple sources
- High-conversion captions for LinkedIn
- AI-generated visuals that fit the post’s tone
- Image + caption merged before upload
- Supports org pages or personal accounts
- Runs on a customizable schedule

## 📁 Folder Structure

```bash
.
├── Linkedin_Automation_with_image_.json  # n8n workflow export
├── README.md
````

## ⚙️ Setup Instructions

1. **Clone this repo**

```bash
git clone https://github.com/<your-username>/linkedin-automation-n8n.git
cd linkedin-automation-n8n
```

2. **Import the workflow**

* Open n8n
* Go to “Workflows” > “Import” and select `Linkedin_Automation_with_image_.json`

3. **Set your credentials**

* LinkedIn OAuth2
* HuggingFace token (for FLUX.1)
* Google Gemini (PaLM/Gemini Pro)

4. **Customize the schedule trigger**
   Set the cron expression in `Schedule Trigger2` to fit your timezone and posting pattern.

5. **Deploy**
   Run it on your local n8n instance or deploy via Docker/N8N Cloud.

## 📬 Output Example

> 🚀 **AUTOMATE LINKEDIN POSTS LIKE A PRO!**
> No more manual formatting, late posting, or content blocks!
> *(Full caption + auto-generated image)*

---

## 🌐 License

MIT — free to use, improve, and contribute.

---

Made with ❤️ using n8n, Gemini, and HuggingFace.

````

---

### 🧠 Steps to Push This to GitHub

1. Create a new repo:
   ```bash
   gh repo create linkedin-automation-n8n --public --source=. --remote=origin
````

2. Initialize git (if not done already):

   ```bash
   git init
   git add .
   git commit -m "Initial commit: LinkedIn Automation with image"
   ```

3. Push to GitHub:

   ```bash
   git remote add origin https://github.com/<your-username>/linkedin-automation-n8n.git
   git branch -M main
   git push -u origin main
