<img src="https://github.com/user-attachments/assets/a839e60b-5537-488f-ac16-c18beca6dcf4" alt="Landscape BrainBloomAI Poster" width="350px">

# BrainBloomAI - Dell InnovateFest 2024

<img src="https://github.com/user-attachments/assets/c887d3a8-08a4-458b-b81b-90abc40f8d0c" alt="3rd Prize Award Photo at Dell Competition" height="220px">

<img src="https://github.com/user-attachments/assets/4d0fb213-c1d0-48f2-a3ce-9f50c549b9b9" alt="Group photo with Minister of Health Mr Ong Ye Kung" height="220px">

<img src="https://github.com/user-attachments/assets/4cc7a88c-40af-4756-8581-91a9b281085b" alt="Group photo with school lecturers and director" height="220px">

**We are proud to share that BrainBloomAI by NYP clinched 3rd Place ($3000 prize) in the prestigious Dell InnovateFest 2024 competition.
The app was showcased before Minister of Health Mr Ong Ye Kung and Mr Eric Chua, Senior Parliamentary Secretary of MCCY on 26th September 2024. 🎉🎉🎉**

BrainBloomAI is an innovative solution targeted to Persons with Intellectual Disabilities (PWIDs), especially those who are clients of [MINDS Singapore](https://www.minds.org.sg/).
The app trains clients' social interaction skills through AI-generated interactions ("games") based in specific settings/backgrounds.

For example, a client can tap on "Retail Customer Service" and play an entirely new on-the-spot AI-generated interaction, role-playing as an employee working at the store who is serving a customer that just walked in.
The AI will play the role of the customer, and will give prompts like "Hi, I'm looking for sneakers. Can you help me?"

Our BrainBloomAI team consists of (in no order):
- [Sarah Zoe Sung](https://github.com/sarahzsu)
- [Chong Cheng Hock](https://github.com/ballgoesvroomvroom)
- [Prakhar Trivedi](https://github.com/Prakhar896)
- [Jun Song](https://github.com/TEOJS12)

Huge thanks to our mentors Mr Alvin Tay, Ms Teo Miow Ting and the support of the school as well!

## Core Features

The game includes features designed specially with PWIDs and MINDS needs in mind.

For PWID clients:
- **Guided repetition**: If the client says something inappropriate, they can re-try and will be even provided an AI-generated guiding prompt to help them come up with a better response
- **Evaluations**: At the end of each game, players will be evaluated based on their performance in their game across standard quantifiable metric domains as well as in a fully-descriptive manner by the AI system. These evaluation criteria are the same as the MINDS Client Evaluation criteria, making it easy to compare and track the progress of clients.
- **Gamification**: Based on how well the client performs in the game, they are rewarded points to encourage them and and incentivise more games. Points can be used to redeem appealing badges.
- **Multi-lingual support**: The app, through Deepgram, supports non-English languages popular in Singapore as well, further catering to a wider user base. Languages supported as of writing include Mandarin, Hindi, Tamil and Malay.

For staff:
- **Custom scenarios**: Scenarios/settings which inspire the AI-generated interactions can be customised entirely. MINDS staff can create new scenarios to help train PWIDs in more specialised/specific areas. This allows the app to be highly adaptible and able to provide comprehensive training.
- **Data-driven approach**: Every single piece of data is tracked, including failed attempts, dialogue information, evaluation data and more. Upon request, staff are also able to export all of a user's data which is automatically sorted, ordered and pre-processed for convenient analysis. This allows MINDS staff, especially client mentees, to help clients much more effectively.
- **Difficuly tuning**: Based on MINDS Client Evaluations keyed in by staff (which also serves as a way to digtise this traditionally paper-backed data), the AI system will automatically tune the difficulty of generated interactions, helping cater more precisely to the client's cognitive abilities and leveling them up from there.

## Let's Get Technical

<img width="960" alt="Solution Architecture" src="https://github.com/user-attachments/assets/92773d7c-ed4c-4665-8020-ae6f5e11f708">

From a more technical perspective, we incorporated several state-of-the-art technologies to deliver a homogeneous user experience:
- Backend
  - `Express.js` API server used by Frontend
    - Core functionality-driving API endpoints
    - Data tracking, storage and management
    - Comprehensive user authentication suite
  - Robust file storage sync with Firebase Cloud Storage
  - Comprehensive AI layer on top of `openai` SDK which can take into account several parameters and configurations
- Speech Service
  - Powerful web socket server using Deepgram AI
  - Used by Frontend to carry out STT/TTS ML
- Frontend
  - `Next.js` web application consolidating services and delivering a user interface
  - Simple, intuitive and clean user interface designed with the user in every step
  - Smooth and short onboarding; users can get started into a game within 1 minute
  - Intuitive game experience, with sound effects, multi-lingual translation, mic input toggling and animation of on-screen dialogues
 
The three core services were containerised into Docker images, uploaded to the Harbor image registry, and deployed to production on RedHat's OpenShift cloud for the competition.

---

Thanks for checking out BrainBloomAI, and we hope you are inspired to look toward a more inclusive future as well! ✨

©️ 2024 BrainBloomAI Team. All rights reserved.
