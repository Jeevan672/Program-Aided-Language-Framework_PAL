# Program-Aided-Language-Framework_PAL
PAL uses CoT reasoning to generate programs in the intermediate reasoning steps
that help solve the given problem. These programs are then passed to an interpreter,
for example, a Python interpreter, that runs the code and returns the result back to
the foundation model (FM).

Similar to ReAct, you need to add one or more examples to the prompt that shows
the model how to format the output. Start each example with a question followed by a
couple of reasoning steps and lines of Python code that solve the problem. Then, add
the new question to solve to the prompt. The PAL-formatted prompt now contains
your example(s) and the new problem to solve

Once you pass this prompt to the FM, the model follows the example and generates
a completion in the form of a Python script. Next, send the script to a Python
interpreter that will run the code and return the result. You can now append the
result to the prompt, and the LLM generates a completion that contains the correct
answer.

![image](https://github.com/Jeevan672/Program-Aided-Language-Framework_PAL/assets/88030873/a4189590-3b65-478b-b8c8-b82ecfeb0404)


Reaearch paper-https://arxiv.org/pdf/2211.10435.pdf
