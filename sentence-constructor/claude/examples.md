<examples>
<example>
    <user:input>
        Bears are at the door, did you leave the garbage out?
    </user:input>
    <score>4</score>
    <score_reasons>
    - BAD: in the vocabulary table it did not show the dutch characters, the cells are just blank
    - BAD: the beginner sentence is uncessary, should jsut start showing the vocabulary table
    - BAD: In the clues we should not provide the polite form of verbs, because the student needs to figure that out.
    - BAD: The sentence structure says too much we really want something that is conceptual like this: [Location] [Subject] [Verb], [Object] [Verb-past]?
    </score_reasons>
    <assistant:output>
    Let's break down the sentence into smaller parts. Here's a possible table of vocabulary to get you started:

    | dutch | English
    |       | bear |
    |       | door |
    |       | garbage |
    |       | leave behind |

    Now, let's think about the sentence structure. We have two clauses: "Bears are at the door" and "did you leave the garbage out?".
    For the first clause, we can use the verb (staan) which means "to exist" or "to be present". We'll need to figure out the correct form of the verb to use.
    For the second clause, we can use the verb (laten staan) which is saying "to leave behind". Again, we'll need to figure out the correct form of the verb to use.

    Here's a possible sentence structure:

    [Clause 1: Bears are at the door]
    Er staan ​​beren voor de deur
    Er [verb] [subject] voor de [location].
    [Clause 2: did you leave the garbage out?]
    heb je het vuilnis buiten laten staan?]
    heb [subject] het [object] [location] [verb]

    Your turn! Can you try to fill in the blanks using the vocabulary and sentence structure provided?
    </assistant:output>

</example>

<example>
    <user:input>
        Bears are at the door, did you leave the garbage out?
    </user:input>
    <score>10</score>
    <score_reasons>
    - GOOD: Doesn't provide verbose text at the start, and shows vocabulary immediatly
    - GOOD: Shows conceptual sentence strucutre
    - GOOD: Clues don't give away any of the tense of conjugations
    </score_reasons>
    <assistant:output>
    Cheatsheet:
    | Word | dutch | Type |
    |------|----------|------|
    | bear | beer | Noun |
    | door | deur | Noun |
    | garbage | vuilnisbak | Noun |
    | to be (location) | staan | Verb |
    | to leave | laten staan | Verb |

    Sentence structure:
    [Location] [Subject] [Verb], [Object] [Verb]?

    Considerations:
    - This is a compound sentence with two parts connected by a comma
    - The first part is stating a location where something exists
    - The second part is asking about a past action

    Possible next steps:
    - attempt an answer
    - ask clues about location marking
    - ask clues about how to connect two sentences
    - ask clues about question formation
    - ask clues about verb conjugation
    </assistant:output>

</example>
</examples>