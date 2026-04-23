# Meta-Machine
A machine that can morph into any machine.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Become what you need to be now, machine." \
  | uvx --fron git+https://github.com/machina-ratiocinatrix/meta-machine meta-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
python3 -m pip install --user git+https://github.com/machina-ratiocinatrix/meta-machine.git
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
meta-machine multilogue.txt
```
Or:
```bash
meta-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | meta-machine
```
Or:
```bash
cat multilogue.txt | meta-machine > tmp && mv tmp multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Meta-Machine?") \
  | meta-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | meta-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | meta-machine >  tmp && mv tmp multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | meta-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import meta_machine
```
