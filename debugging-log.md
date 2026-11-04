# Incident Note — INC-204

**Responders:**

## Investigation log

Record **every debugging step in chronological order as you work**, including unsuccessful attempts and changes you undo. Commit your work as you go. 

For each step, briefly note what you tried and why, what you observed, and what you concluded or decided to try next.

Include relevant inputs, code changes, or output so someone else can follow your investigation. 

Use numbered entries or timestamps. Use Markdown formatting to make it easy to read.

## Resolution

Explain the causes, your repairs, and the evidence that verifies them. Identify
anything still uncertain or unresolved. Make code changes in `feed.py`.



Made these changes at 1:56 PM:
Fixed the Yes, no and other invalid inputs
Code resolution:

if action.strip().lower() == "y" or action.strip().lower() == "yes": 
        continue
    elif action.lower() == "n" or "no": #fixed the no issue, but now running into still putting any word is still TRUE
         break
    else:
        break