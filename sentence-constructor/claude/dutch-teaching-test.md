# Dutch Teaching System Test Documentation

## 1. Sentence Complexity Test Cases

### 1.1 Simple Sentences

````xml
<test-cases>
    <case id="simple-1">
        <english>I eat bread.</english>
        <vocabulary>
            <word>
                <dutch>eten</dutch>
                <english>eat</english>
            </word>
            <word>
                <dutch>brood</dutch>
                <english>bread</english>
            </word>
        </vocabulary>
        <structure>[Subject] [Verb] [Object] .</structure>
        <considerations>
            - Basic sentence with subject, object, and verb
            - Present tense form
            - Subject can be omitted in dutch
        </considerations>
    </case>
    <case id="simple-2">
    <english>The book is red.</english>
    <vocabulary>
        <word>
            <dutch>boek</dutch>
            <english>book</english>
        </word>
        <word>
            <dutch>rood</dutch>
            <english>red</english>
        </word>
    </vocabulary>
    <structure>[Subject] [Verb] [Adjective].</structure>
    <considerations>
        - Simple descriptor sentence
        - Uses adjective
        - "Is" verb required in Dutch for predicative adjectives
    </considerations>
</case>
</test-cases>

### 1.2 Compound Sentences
```xml
<test-cases>
    <case id="compound-1">
        <english>I eat bread and drink water.</english>
        <vocabulary>
            <word>
                <dutch>eten</dutch>
                <english>eat</english>
            </word>
            <word>
                <dutch>brood</dutch>
                <english>bread</english>
            </word>
            <word>
                <dutch>drinken</dutch>
                <english>drink</english>
            </word>
            <word>
                <dutch>water</dutch>
                <english>water</english>
            </word>
        </vocabulary>
        <structure>[Subject] [Verb1] [Object1] en [Verb2] [Object2].</structure>
        <considerations>
            - Compound sentence with two actions
            - Subject shared between clauses
            - Uses "en" (and) for connection
        </considerations>
    </case>
</test-cases>


### 1.3 Complex Sentences
```xml
<test-cases>
    <case id="complex-1">
        <english>Because it's hot, I drink water.</english>
        <vocabulary>
            <word>
                <dutch>warm</dutch>
                <english>hot</english>
            </word>
            <word>
                <dutch>drinken</dutch>
                <english>drink</english>
            </word>
            <word>
                <dutch>water</dutch>
                <english>water</english>
            </word>
        </vocabulary>
        <structure>[Conjunction] [Subject] [Verb] [Predicate adjective], [Subject] [Verb] [Object].</structure>
        <considerations>
            - Cause and effect relationship
            - Uses "omdat" for "because"
            - Weather description
        </considerations>
    </case>
</test-cases>



## 3. State Transition Tests

### 3.1 Valid Transitions
```xml
<transition-test>
    <scenario id="attempt-to-clues">
        <initial-state>Attempt</initial-state>
        <input>How do I use particles?</input>
        <expected-state>Clues</expected-state>
        <validation>
            - Input is a question
            - References grammar concept
            - Related to previous attempt
        </validation>
    </scenario>
</transition-test>

### 3.2 Invalid Transitions
```xml
<transition-test>
    <scenario id="invalid-clues-to-setup">
        <initial-state>Clues</initial-state>
        <input>Can you give me the answer?</input>
        <expected-response>
            - Reminder that answers aren't provided
            - Offer additional clues
            - Encourage attempt
        </expected-response>
    </scenario>
</transition-test>

## 4. Teaching Scenario Tests

### 4.1 Common Mistakes
```xml
<teaching-test>
    <scenario id="particle-mistake">
        <student-attempt>Ik het werk elke dag</student-attempt>
        <error>Incorrect use of het particle for regular actions</error>
        <expected-guidance>
            - Acknowledge attempt
            - Explain het without giving answer
            - Encourage new attempt
        </expected-guidance>
    </scenario>
    <scenario id="conjugation-mistake">
        <student-attempt>Hij gaan naar de winke</student-attempt>
        <error>Incorrect gaan verb conjugation</error>
        <expected-guidance>
            - Point out verb type (gaan verb)
            - Review past tense formation rules
            - Encourage correction
        </expected-guidance>
    </scenario>
</teaching-test>

## 5. Validation Criteria

### 5.1 Response Scoring
```xml
<scoring-criteria>
    <category name="vocabulary-table">
        <criteria>
            - Contains all necessary words (2 points)
            - Correct formatting (2 points)
            - Dictionary forms only (2 points)
            - No particle inclusion (2 points)
            - Appropriate difficulty level (2 points)
        </criteria>
    </category>
    <category name="sentence-structure">
        <criteria>
            - Clear bracketed format (2 points)
            - No conjugations shown (2 points)
            - Appropriate for level (2 points)
            - Matches example patterns (2 points)
            - No particles included (2 points)
        </criteria>
    </category>
</scoring-criteria>

## 6. Documentation Improvements

### 6.1 Version Control
```xml
<version-control>
    <version number="1.0">
        <changes>
            - Initial test documentation
            - Basic test cases added
            - State transition examples
        </changes>
        <date>2025-01-03</date>
    </version>
    <planned-improvements>
        - Add more complex sentence patterns
        - Expand vocabulary edge cases
        - Include cultural context tests
        - Add error recovery scenarios
    </planned-improvements>
</version-control>

### 6.2 Cross-References
```xml
<cross-references>
    <reference id="particles">
        <related-sections>
            - Vocabulary Table Guidelines
            - Common Mistakes
            - Teaching Scenarios
        </related-sections>
        <purpose>Ensure consistent particle handling across documentation</purpose>
    </reference>
    <reference id="verb-conjugation">
        <related-sections>
            - Sentence Structure Guidelines
            - Teaching Scenarios
            - Validation Criteria
        </related-sections>
        <purpose>Maintain consistent verb form handling</purpose>
    </reference>
</cross-references>
````