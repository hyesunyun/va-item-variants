# Prompts for Large Language Models (LLMs)

We used GPT-3 and ChatGPT to generate the questionnaire item variants and various conversation content for the agent. We attempted various prompting strategies before finalizing the prompts. In our study, we used the hyperparameters `temperature = 0.7` and `top_p = 1` for GPT-3 model as we saw the best results despite some duplicate outputs when we made up to 20 requests per prompt. The actual prompts we used for the study are provided below.

## Prompts for Generating Item Variants

**GPT-3**
```
Statement: {{ORIGINAL ITEM}}

Ask the above statement as a long question. Also, change the time from past 7 days to from yesterday. The answer of the question should be between: Never, Rarely, Sometimes, Often, Always.

Question:
```

**ChatGPT**
```
Statement: {{ORIGINAL ITEM}}

Give me ten different conversational questions which try to measure the same concept in the statement. Also, ask it from yesterday or since the last time we talked. 

The question should be formatted for the following answers only: Never, Rarely, Sometimes, Often, Always.
```

## Prompts for Generating Stories

For generating personal anecdotes, we chose 15 general everyday topics to prompt the LLMs. The 15 topics were: `grocery shopping`, `commuting to work`, `having lunch`, `making dinner`, `going to a party with a friend`, 
`watching a basketball game`, `trying a new restaurant the past weekend`, `reading a new book`, `going to a live theatre show`, `hosting a potluck`, `having a boring day at work`, `spilling coffee all over the place while getting ready for work`, `feeling a bit under the weather`, `going to the dentist`, and `going for a hike`.

**GPT-3**
```
Give an engaging, interesting first-person story of a character on the topic of {{TOPIC}} that can be shared with someone in 3 sentences.
```

**ChatGPT**
```
Marie is a character who is responsible for asking different questions of other people's mood and depression symptoms. Please give me a backstory for Marie in first person.
```

## Prompts for Generating Jokes

**GPT-3**
```
Marie is a computer-animated agent who is responsible for asking different questions of the user's mood and depression symptoms. She asks serious questions every day and would like to use humor to make the conversation more engaging and uplifting. What joke should Marie tell?
```

```
What funny joke can I tell to make a very serious conversation more uplifting?
```

```
Give a short joke that a mental health counselor can tell to a patient.
```

**GPT-3 & ChatGPT**
```
Tell me a short joke.
```

```
Tell me a really funny computer-related joke.
```

```
Give me a joke about computer-animated character.
```

## Prompts for Generating Empathetic Responses

The `{{ORIGINAL ITEM CONTENT}}` refers to the main content of the original question or item. For example: if the original item is `In the past 7 days, I felt worthless.`, we would prompt the model with `Provide a short empathetic response for someone who never or rarely feels worthless.`

**GPT-3 & ChatGPT**
```
Provide a short empathetic response for someone who never or rarely feels {{ORIGINAL ITEM CONTENT}}
```

```
Provide a short empathetic response for someone who often or always feels {{ORIGINAL ITEM CONTENT}}
```

```
Provide a short empathetic response for someone who sometimes feels {{ORIGINAL ITEM CONTENT}}
```

## Prompts for Generating Motivating Messages

**GPT-3 & ChatGPT**
```
Give me a short inspiring message for the day.
```

```
Share a short uplifting quote for me.
```

## Prompts for Generating Farewells

**GPT-3 & ChatGPT**
```
What can I tell someone to signal an end to a conversation before saying goodbye?
```

```
How can I end a conversation in a nice way before saying goodbye to someone who I was talking to?
```

```
Marie is a character who meets someone and has had a good conversation. Give me a short thing that Marie should say before saying goodbye in first person.
```

```
I am feeling very low and down today. Give me a short uplifting message.
```

```
Marie is a character whose job is to only check in on different clients' moods and feelings and does not provide advice. Give me a short script that Marie can use before saying goodbye to one of her clients in first person.
```