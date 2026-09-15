# bus-4040-week-3-homework-quiz-sim

## What type of quiz did I create

A 20-question self-test covering weeks 1-3 of BUS 4040: GitHub and version
control basics (Git history, branches, README/main branch setup, HTTPS auth)
and the AI fundamentals from week 3 (model tiers, tokens, context windows,
harnesses, open weight vs. closed models). It's a mix of multiple choice and
true/false, one question at a time, shuffled on every run. It's a single
`index.html` file - no server, no internet connection, nothing to install.
Double-click it and it just works.

## What worked

Giving the AI a detailed one-shot prompt (source material, exact output
format, exact quiz behavior) got me a fully working quiz on the first try -
no follow-up fixes needed to the code itself. I ran it end to end afterward:
first pass I scored 17/20, missed 3 questions, hit "retry just the missed
ones" and it correctly gave me only those 3, got that down to 1, retried
again, and got a "perfect round" message. The retry-only-what-you-missed
feature worked exactly like I wanted, which was the part I was least sure
would come out right from a single prompt.

## What did not work / adjustments I made

The code itself didn't need debugging, but I did have to slow down and
actually check the questions against the source files line by line. It's
easy to assume AI got everything right because it sounds confident, so I
made sure every question and explanation traced back to something the
narrative or homework files literally said, rather than something that just
sounded plausible. The other real friction wasn't the quiz logic at all - it
was getting files to save correctly through Git Bash (paste kept breaking in
weird ways), which had nothing to do with the AI-generated content and
everything to do with terminal quirks on my machine.

## How I could apply this to other activities

This is basically a recipe for turning any reference material I already
have into a self-check tool - I could do the same thing with training
material at my internship, a study guide for another class, or even
onboarding notes for a new hire at Narrow Road. The pattern is: be specific
about the source material (don't let it invent facts), be specific about
the exact behavior you want, and then actually test the output yourself
instead of assuming a one-shot prompt got everything right.
