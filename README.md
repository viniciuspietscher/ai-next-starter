# Next.js OpenAI Starter App

This is a starter kit for integrating [OpenAI's API](https://platform.openai.com/docs/api-reference) into a [Next.js](https://nextjs.org/) application. It is crafted with minimal styling and basic API integration so you can strip it and bring your own libraries to make it your own. Feel free to fork and create something amazing!

## Getting Started

First, fork the repo to your dev environment and install the packages:

```bash
npm i
```

Then, run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Important!

Make sure that update the `OPENAI_API_KEY=yourApiKey` in the `.env` file.

## Workshop 1:
This was the fun starting point. During this workshop we familiarized ourself with the Playground and how it needs to be used, where do we enter our prompts and how AI can return response in a JSON object format. We also learnt how we we need to provide our prompts, they need to be specific to get desired answer. Also AI was smart enough to take the previous prompt output into the next prompt.
-Create a fictitious company or organization: We all agreed to make an app related to mental health so we asked AI to suggest some with this 
  PROMPT_1: "We need your assistance in creating Mental Health app so it can track mental state and provide coping strategies. Please return a json object that we can use later in an application."
  ASSISTANT: Returned a starting point for creating Mental Health app with a JSON object which keeps track of various parameters like        users, mood, therapy sessions, coping strategies etc.
  PROMPT_2: "Please suggest the name for the app, it's mission and values and then return the json object that you can use later in an application"
  ASSISTANT: 
  {
    "appName": "MindWave",
    "mission": "To provide a supportive tool for managing mental health, promoting self-awareness, and encouraging healthy coping strategies.",
    "values": [
        "Compassion",
        "Empathy",
        "Wellness",
        "Privacy",
        "Accessibility"
    ],
    },
    PROMPT_3: Using this json object as a company descriptor:{above JSON object} produce 20 product reviews for the product some of which are positive some of which are negative. Have them returned in an array we can use later."
    ASSISTANT: This returned 20 reviews with id, rating and comment.
    PROMPT_4:
    ASSISTANT: This is the object we received.
    {
    "positive_sentiment": 12,
    "negative_sentiment": 8,
    "summary": "Overall, users have a positive view towards 'MindWave' as reflected in a majority of the reviews. They appreciate its       functionality in managing mental health and its feature of providing coping strategies. Some users, however, reported technical         issues with the app including crashes and a confusing interface. These areas of improvement have been duly noted."
    }
    
    
    
