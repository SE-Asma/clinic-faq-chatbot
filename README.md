# Clinic FAQ Chatbot (Healthcare AI)

An AI-powered receptionist chatbot for aesthetic and skin clinics, built in Python with Google's Gemini large language model.

Patients can ask about opening hours, treatments, prices, booking and aftercare. The bot answers **only from the clinic's own information** and politely refers anything else to the clinic team, so it does not make up prices or medical details.

## Features
- Answers patient questions in natural, friendly language
- Grounded answers: uses only the clinic's provided information (reduces hallucinations)
- Safe fallback: unknown questions are passed to the clinic team
- Interactive chat loop (type `bye` to end)
- API key stored securely in Colab Secrets, never in the code

## Tech stack
- Python
- Google Gemini API (`google-genai`)
- Google Colab

## Example
```
You: How much is a HydraFacial?
Bot: A HydraFacial is £95. Let me know if you'd like to book!

You: Do you offer laser hair removal?
Bot: We don't currently have that listed in our treatments. I'll check with the team. You're welcome to call us on 0161 000 0000.
```

## How to run
1. Open `clinic_chatbot.ipynb` in Google Colab (link at the top of the notebook).
2. Create a free Gemini API key at https://aistudio.google.com and add it in Colab under **Secrets** as `GEMINI_API_KEY`.
3. Run the cells from top to bottom.

## Next steps
- Load clinic information from a file or website
- Add appointment booking via a form or calendar
- Deploy as a web chat widget

*Note: the clinic details used here are fictional, for demonstration purposes.*

---
Built by **Asma Tahir** · [Portfolio](https://asmatahir.surge.sh) · [LinkedIn](https://www.linkedin.com/in/asmatahirwebdev11052001)
