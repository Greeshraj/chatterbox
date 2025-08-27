### Chatterbox Application: Simple System Design Document

**I am Greeshraj Patairiya, a 5th-year undergraduate student at the Indian Institute of Technology Kharagpur.**

---

#### **1. Overview**

**Chatterbox** is a messaging app where users can chat with friends, either one-on-one or in groups. It also has an AI tool that responds to messages starting with `@bot`. The app supports text messages and video calls.

---

#### **2. Technology Used**

- **Next.js (App Router):** Framework for building the app.
- **Convex:** Handles the database, real-time updates, and cloud functions.
- **ShadCN:** Provides ready-made UI components.
- **Convex File Storage:** Stores images and videos.
- **ZegoCloud:** Manages video calls.
- **Clerk:** Handles user logins and accounts.
- **Tailwind CSS:** Used for styling the app.
- **TypeScript:** Adds type safety to the code.

---

#### **3. How It Works**

1. **User Login:**  
   Users log in with Clerk, which manages their account and session.

2. **Chatting:**  
   Users send messages that are stored in Convex and updated in real-time for everyone in the chat.

3. **Using AI:**  
   Type `@bot` before your message to get a response from the AI tool, powered by OpenAI.

4. **Sharing Files:**  
   Users can share images and videos, which are stored in Convex File Storage.

5. **Video Calls:**  
   Users can start video calls through ZegoCloud.

---

#### **4. How to Set Up**

1. **Install Dependencies:**
   - Run `npm install` to install everything needed.

2. **Set Up Convex:**
   - Run `npm run dev` to log in to Convex and create a project.

3. **Set Up Clerk:**
   - Create a Clerk account and get the necessary keys. Add them to your `.env.local` file. ("If you don't want to get into the details, just ping me, and I'll share the env file with you with you.")

4. **Set Up OpenAI:**
   - Get your OpenAI API key and add it to Convex's environment variables.

5. **Set Up ZegoCloud:**
   - Create a ZegoCloud account for video calls. Add the required keys to your `.env.local` file.

6. **Run the App:**
   - Start the app with `npm run dev`. 
   - Open new terminal /powershell and run with `npx convex dev`. The app should now be running locally.
   - Keep in mind when you run the convex server, dont close it, keep it running.

---

#### **5. Why These Technologies?**

- **Next.js** makes it easy to build and deploy web apps.
- **Convex** simplifies database management and real-time updates.
- **Clerk** handles user login without extra coding.
- **ZegoCloud** provides easy video call integration.
- **Tailwind CSS** makes styling fast and flexible.
- **TypeScript** catches errors early and makes the code more reliable.

---
