# Conversational Artificial Intelligence (AI)

## The Turing Test

> The **Turing test**, originally called the **imitation game** by [Alan Turing](https://en.wikipedia.org/wiki/Alan_Turing) in 1950,[[2\]](https://en.wikipedia.org/wiki/Turing_test#cite_note-Turing-1950-2) is a test of a machine's ability to [exhibit intelligent behaviour](https://en.wikipedia.org/wiki/Artificial_intelligence) equivalent to, or indistinguishable from, that of a human. Turing proposed that a human evaluator would judge natural language conversations between a human and a machine designed to generate human-like responses. The evaluator would be aware that one of the two partners in conversation is a machine, and all participants would be separated from one another. The conversation would be limited to a text-only channel such as a computer keyboard and screen so the result would not depend on the machine's ability to render words as speech.[[3\]](https://en.wikipedia.org/wiki/Turing_test#cite_note-3) If the evaluator cannot reliably tell the machine from the human, the machine is said to have passed the test. The test results do not depend on the machine's ability to give correct [answers to questions](https://en.wikipedia.org/wiki/Question_answering), only how closely its answers resemble those a human would give.

## Types

1. Rule Based chat-bots

   - One-Turn interaction

   - Use predefined rules (conditional statements) for responding to conversation

   - Can be easily confused

   - Almost always fail the Turing Test

     - Exception:  

       > **Eugene Goostman** is a [chatbot](https://en.wikipedia.org/wiki/Chatbot) that some regard as having passed the [Turing test](https://en.wikipedia.org/wiki/Turing_test), a test of a computer's ability to communicate indistinguishably from a human. Developed in [Saint Petersburg](https://en.wikipedia.org/wiki/Saint_Petersburg) in 2001 by a group of three programmers, the Russian-born Vladimir Veselov, Ukrainian-born Eugene Demchenko, and Russian-born Sergey Ulasen,[[1\]](https://en.wikipedia.org/wiki/Eugene_Goostman#cite_note-zdnet-eugenepass-1)[[2\]](https://en.wikipedia.org/wiki/Eugene_Goostman#cite_note-uor-success-2) Goostman is portrayed as a 13-year-old Ukrainian boy—characteristics that are intended to induce forgiveness in those with whom it interacts for its grammatical errors and lack of general knowledge.

2. Intelligent Virtual Assistants

   - Multi-turn interactions (it remembers past interactions)
   - Can be used for general "content generation"
   - Use neural-network models for natural language processing
   - Can frequently pass the Turing test unless the test is clever or bizarre
   - Current best example: GPT-3

## How Does GPT-3 Work?

- Main idea: predict one word at a time, using the previous words as a pattern
- Has over 175 Billion parameters
- Trained on data collected from internet:
  - Books
  - News articles
  - Blog posts
- Users supply GPT-3 with a "prompt" and it generates output
- Output is randomly generated using combinations of the training data is was created with

## What is wrong with GPT-3?

- GPT-3 very often will produce offensive, toxic, or false statements
- The main reason is because it is using "the Internet" as it's training data
  - "It's holding up a mirror"

## What can be done about it?

- Lots of people are trying lots of things:
  - Prompt with something positive: "The good bot said:"
  - Use another bot to filter the output, keeping the bad stuff out
    - This requires yet another level of automation!
    - Doesn't ever seem to work 100%
  - Use humans to filter the output
    - Seen as the safest option for now, but uses expensive human labor
  - Use better training data
    - If the training data doesn't contain offensive stuff, then the model has a better chance of being clean
    - Timnit Gebru and Google AI
      - Timnit's paper outlined 4 concerns with these types of models:
        - Environmental costs: training the models is absurdly power intensive (same amount of pollution as a round-trip flight from SFO to New York for one train)
        - Data set is too large and uncontrollable (auditing it is REALLY hard)
        - Research dollars are NOT being spent on other avenues of potential success
        - The models can easily fool people