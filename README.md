# Avalanche Methodology

A stab at a post-AI dev process model. Most of the Agile techniques still hold as best known practices, but they need a major shake-up. "Avalanche", because there are characteristics in common with the [Waterfall model](https://en.wikipedia.org/wiki/Waterfall_model), only it's much, much more chaotic.

**Status 2025-06-20 :** This repo created. I have loads of scattered notes on this machine to review, but I have jotted some key points down with pen & paper, transcribed below.

Below is a **Workflow Sequence** I've found myself using. This is evolving all the time, so this can only seen as a snapshot. The section below it **Praxis** has suggestions on implementation of the process. **Observations** is an attempt to capture potential causes of problems and how to mitigate them.

## Workflow Sequence

This sequence is only a general guideline structure, not a binding contract. It should be **adapted** for your own particular requirements and resources, or **ignored** entirely.

#### 1. Ideate
<details>
  <summary>Think about what you want to achieve...</summary>
  <p>as you might traditionally, with brainstorming, pondering on a dog walk etc. Keeping plans realistic used to be a problem, every developer has has their fingers burnt. But now the rules have changed - **Think Big!** Don't fear being over-ambitious.</p>
</details>

#### 2. Forage
<details>
  <summary>Collect all the existing material you can find related to the idea.</summary>
  <p>Time spent on research has always had value; reuse of existing code has always saved time. *On the shoulders of...* Now LLMs can interpret pretty much anything, the value of foraging has gone up orders of magnitude. Give a plan-mode assistant a couple of academic papers about a system, get it to create a strategy for implementation.
    Say there's a lib you would like to use in your project, except it's in Python and you're using Javascript. Simply have a code assistant port it. *This works best for smallish projects. For a particular tool I did exactly this. First I got Claude to help me write a detailed system prompt describing the target system/libs/style. Then used [Repomix](https://repomix.com/) to package up the Python codebase and stuck these in a Claude Project. The first pass was near enough to be able to take to VS Code and quasi-manually get working. Very few hours.*</p>
</details>

#### 3. Plan Overall Architecture (human)

#### 4. Plan (AI)

#### 5. Build

#### 6. Consolidate

#### 7. Pivot

## Praxis

_**if in doubt, include a timeout**_

### Learning Exercise
fail a lot
### Multitask
### Experiment
### Throw Things Away
Dev is cheap
### Encourage Feedback Loops
### Rapid Activity Switching
### Experiment
### Keep Track
pay attention
### Freeze, Reuse
### Feature Flags
### Design for Serendipity

## Observations

* **AI assistants are opinionated**
Code assistant LLMs owe a lot of their knowledge to the archives of sites like Stack Overflow and Reddit. One these sites, for every correct response to a question there are 4 broken ones. This knowledge favours the technologies used at the time. The reality of using archive material for training means **it will always be legacy**.  
**Workaround :** create a **comprehensive system prompt** detailing the technologies and tools you want to use in your project.  

* **Cognitive debt accumulates**
Where the thing you have built has gone way beyond your initial conception and you haven't a clue what it can do. **Workaround :** If you feel lost at sea, **ask your assistant for a tutorial**.

* **LLMs don't suffer from Impostor Syndrome**
Their strategy is more "fake it til you make it", backed up with flattery. 
