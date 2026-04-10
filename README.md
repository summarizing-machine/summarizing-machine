# Summarizing-Machine
A Machine that summarizes texts.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx summarizing-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install summarizing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
summarizing-machine multilogue.txt
```
Or:
```bash
summarizing-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | summarizing-machine
```
Or:
```bash
cat multilogue.txt | summarizing-machine > multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Summarizing-Machine?") \
  | summarizing-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | summarizing-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | summarizing-machine > multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | analyzing-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import thinking_machine
```
