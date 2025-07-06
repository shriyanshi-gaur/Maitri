# 🤱🧠 Maitri – AI Assistant for Maternal Health & Mental Wellness

**Maitri** (मैत्री) is an empathetic, LLM-powered AI assistant designed to support **pregnant women**, **young mothers**, and **caregivers** by providing science-backed, compassionate guidance around **maternal nutrition**, **pregnancy care**, **postpartum health**, and **mental well-being**.

Built using **LangChain**, **ChromaDB**, **Groq's LLaMA-3**, and deployed with **Gradio**, Maitri can answer nuanced, emotionally sensitive queries while retrieving accurate information from medical literature.

📚 Source Materials Used
All responses by Maitri are generated using trusted, preloaded PDF documents related to maternal health, nutrition, and mental wellness. These documents are stored in the /data/ folder and embedded using ChromaDB.

| Document Title                                    | Domain             | Source                |
| ------------------------------------------------- | ------------------ | --------------------- |
| *Handbook of Nutrition and Pregnancy*             | Maternal Nutrition | Springer              |
| *Essentials of Maternal and Child Health Nursing* | Pregnancy Care     | Open Nursing Texts    |
| *Mental Health Handbook (Clinical Psychology)*    | Mental Wellness    | Public Health Archive |
| *WHO Guidelines on Postnatal Care*                | Maternal & Infant  | WHO Docs              |


✅ You can add more PDF documents by placing them inside the /data/ folder and rerunning the vector database generation script.



---

## 🌟 Features

- ✅ **Personalized Q&A** based on real clinical content
- ✅ Retrieval-Augmented Generation (RAG) using ChromaDB
- ✅ Powered by **Groq’s LLaMA-3 70B** for fast, intelligent responses
- ✅ Soft, maternal UI with **Gradio**
- ✅ Responds with warmth, evidence, and clarity — no hallucinations
- ✅ Supports **complex, emotionally sensitive questions**  
- 🔒 Privacy-first: No data is stored or shared

---

## 🧠 Example User Query

> “I’m in my third trimester and constantly anxious about childbirth. I’ve read so many things online, I feel overwhelmed. How can I manage these fears while taking care of myself nutritionally?”

**📎 Maitri’s Response** (example):



🤱 AI Assistant for Maternal & Child Health is ready!

👩‍🍼 Ask a question:  “I’m in my third trimester and constantly anxious about childbirth. I’ve read so many things online, I feel overwhelmed. How can I manage these fears while taking care of myself nutritionally?”

🤖 Maitri AI:
I completely understand your concerns, and it's great that you're thinking about your well-being during this time. According to the American College of Obstetricians and Gynecologists (ACOG), it's normal to feel anxious or overwhelmed during pregnancy, especially when it comes to childbirth.

To manage your fears, ACOG suggests the following:

1. **Education is key**: Learning about the childbirth process and what to expect can help alleviate fears. Consider taking a childbirth education class or talking to your healthcare provider about your concerns.
2. **Breathing exercises and relaxation techniques**: Deep breathing, meditation, and yoga can help you relax and reduce anxiety. You can find many guided relaxation exercises online or through mobile apps.
3. **Support system**: Surround yourself with a supportive partner, family, and friends. Sharing your feelings with them can help you feel more connected and less anxious.

Now, let's talk about nutrition! A well-balanced diet is essential for your health and your baby's growth. ACOG recommends:

1. **Eat a variety of foods**: Focus on whole, nutrient-dense foods like fruits, vegetables, whole grains, lean proteins, and healthy fats. Aim for a rainbow of colors on your plate to ensure you're getting a range of vitamins and minerals.
2. **Stay hydrated**: Drink plenty of water throughout the day to help your body function properly and support your baby's growth.
3. **Calcium and vitamin D**: These nutrients are crucial for your baby's bone development. You can find them in foods like dairy products, leafy greens, and fortified cereals.

Remember, it's essential to talk to your healthcare provider about your specific nutritional needs and any concerns you may have. They can provide personalized guidance and support.

Lastly, don't hesitate to reach out to your healthcare provider if your anxiety becomes overwhelming or interferes with your daily life. They're there to support you throughout your pregnancy journey.

I hope this helps you feel more empowered and in control, mama!









👩‍🍼 Ask a question: “I live in a remote area and feel isolated after my delivery. I can’t talk to anyone and cry often. Could this be postpartum depression, and how do I keep myself and my newborn healthy during this time?”

🤖 Maitri AI:
I'm so sorry to hear you're feeling isolated and overwhelmed after your delivery. It's completely normal to experience a range of emotions during this time, and it's great that you're reaching out for support.

According to the World Health Organization (WHO), postpartum depression (PPD) is a common condition that affects many new mothers. It's characterized by feelings of sadness, anxiety, and hopelessness that can make it difficult to care for yourself and your baby.

Some common symptoms of PPD include:

* Feeling sad, empty, or hopeless
* Crying often
* Difficulty sleeping or eating
* Feeling anxious or irritable
* Difficulty bonding with your baby
* Feeling guilty or worthless

If you're experiencing some or all of these symptoms, it's essential to reach out to a healthcare provider for support. They can help you develop a plan to manage your symptoms and ensure you and your baby receive the care you need.

In the meantime, here are some tips to help you cope with PPD and keep yourself and your newborn healthy:

1. **Reach out to a trusted friend or family member**: Even if you can't talk to someone in person, try to connect with a loved one over the phone or video call. Sharing your feelings with someone you trust can help you feel less alone.
2. **Join a support group**: Look for online support groups or forums where you can connect with other new mothers who may be experiencing similar feelings.
3. **Take care of your physical health**: Make sure to eat nutritious foods, stay hydrated, and get plenty of rest. This can help improve your mood and energy levels.
4. **Prioritize self-care**: Take breaks when you need them, and do things that bring you joy and relaxation, like reading a book or taking a warm bath.
5. **Bond with your baby**: Skin-to-skin contact, breastfeeding, and gentle massage can help you bond with your baby and reduce feelings of anxiety and depression.

Remember, you're not alone, and it's okay to ask for help. Your healthcare provider can connect you with local resources and support services to help you manage PPD.

Keep in mind that PPD is a treatable condition, and with the right support, you can feel better and care for your newborn with confidence.

Source:
World Health Organization. (2018). Postpartum care. Retrieved from <https://www.who.int/news-room/fact-sheets/detail/postpartum-care>


| Capability                       | Covered   |
| ---------------------------------| --------- |
| 🧠 Empathy & reassurance         | ✅       |
| 📚 Clinical knowledge            | ✅       |
| 🧮 Emotional + dietary reasoning | ✅       |
| 🌍 Cultural sensitivity          | ✅       |
| 🧘 Self-care advice              | ✅       |


---

## 🛠️ Tech Stack

| Component     | Tool/Library                             |
|---------------|------------------------------------------|
| LLM           | Groq’s LLaMA-3 (via LangChain)           |
| Embeddings    | `sentence-transformers/all-MiniLM-L6-v2` |
| Retrieval     | ChromaDB                                 |
| PDF Parsing   | PyPDFLoader                              |
| UI            | Gradio                                   |
| Framework     | LangChain (RetrievalQA)                  |
| Language      | Python                                   |

---


## 🚀 Run Locally (Colab or Terminal)

```bash
pip install langchain langchain-community chromadb gradio sentence-transformers
python maitri_chatbot.py


📌 Disclaimer
Maitri is NOT a replacement for professional medical or psychological care.
It is an educational assistant based on clinical documents and should only be used as a first step toward informed support.
---

🙌 Credits
Built with 💙 for maternal and mental health equity.
By [Shriyanshi Gaur]



