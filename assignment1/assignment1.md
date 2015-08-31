<p style='text-align: center;'><b>Ronald Allison</b></p>
<p style='text-align: center;'><b>CS 7637 Assignment 1</b></p>
<p style='text-align: center;'><b>Use Of Semantic Networks In A Cognative System That Takes The Raven's Progressive Matrices Intellegence Test</b></p>


# Introduction and Abstract

The Raven's Progressive Matrices test (RPM) is an intelligence test that consists of 60 questions, where each question is presented to the test-taker in visual format.  Each question consists of a logical sequence of geometric symbols, and the test-taker must select, from multiple choices, the correct missing element that successfully completes the pattern.  We will herein design a cognative system    (KBAI agent) that uses semantic networks to organize, store and otherwise represent the knowledge necessary for an agent to read, reason about and answer an RPM question. 

Note that the RPM tests has no letters and no numbers, only logical sequences expressed through geometric symbols.  Therefore the process of answering  answering a given RPM question, whether the test-taker is human or computer, generally involves:
- interpreting and encoding the information contained in the question
- analyzing the information 
- selecting and outputting the (hopefully correct) answer

We will use semantic networks to represent the information contained in a given question in a form that the agent can utilize to reason about the question and ultimately output an answer.  The semantic networks consists of objects which we will categorize as geometric shapes, and transformations that these shapes may undergo.  We will represent the shapes and the transformations that the shapes may undergo as nodes and vertices, respectively.  Thus we will encode the information in a given RPM question in an organized way such that the agent may reason about the question, or analyze the information, using several different non-mutually exclusive options such as [situational calculus](https://en.wikipedia.org/wiki/Situation_calculus), [directed graph logic](https://en.wikipedia.org/wiki/Directed_graph), etc. in order to deliberate, metacognate and output the best answer.  

Note that agent deliberation and agent metacognition details/algorithms are not directly addressed here, rather we are focused on describing a suitable knowledge representation scheme.  However it is important to note that during metacognition, which for our agent occurs upon learning the results of its guess for a given question, the semantic network once again comes into play in that the agent could make changes to the semantic network (nodes and/or vertices of the directed graph).  That is, given new information the agent may decide to alter its belief system, which may entail altering the semantic network that it is using to encode the same.  

# Steps
1. Read in the question (either images or verbal representation of the images
(the question).
2. Interpret (if necessary) and store the information using nodes to represent
the objects (or lack thereof) in each question frame.
3. Interpret and store the relationships between the objects, useing vertices
to represent the relationships between the objects, where the vertices are
labled with the transformation that the object may have undergone e.g., expanded,
unchanged, deleted, etc. 
4. Read in the potential answers, interpreting and storing the objects and their
relationships for each answer.
5. Deliberate and select an answer.
6. Output the answer.
7. Learn whether or not the answer was correct.
8. Potentially update the agent's belief system, which may include updating the
semantic network representation, based on the feedback.


