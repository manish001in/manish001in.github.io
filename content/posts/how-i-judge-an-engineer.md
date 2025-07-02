+++
date = "2025-07-02"
title = "How I Judge an Engineer: It's All About Depth"
description = "The one question that reveals everything about a developer's potential: How deep do they go when they don't know something?"
+++


*The difference between good and great engineers isn't what they know - it's how they figure out what they don't know.*

---

## The Question That Reveals Everything

After having a fair bit of experience building software and working with dozens of engineers across startups and established companies, I've developed a simple heuristic for evaluating technical potential. It's not about years of experience, prestigious companies, or even the complexity of projects they've worked on.

**It's about how deep they go when they encounter something they don't understand.**

This single trait tells me more about an engineer's potential than any algorithm quiz or system design interview ever could.

## The Stack Overflow Test

Don't get me wrong - Stack Overflow is an incredible resource. I've used it countless times, and it's saved me hours of debugging. But here's the thing: how someone <u>uses</u> Stack Overflow reveals everything about their approach to problem-solving.

## Stack Overflow is dead gramps, what about the new fancy LLMs?

LLMs are great. I love them. I use them every day. They can give you a fairly correct answer to anything you search for. But did you try to understand the answer? Did you ask ChatGPT or Claude or Gemini to explain the answer? Learn about the nitty gritties?

What's the point of having all the knowledge in the world if you don't know how to use it or don't understand why a particular solution works?


### **The Surface-Level Engineer**
- Hits a problem → immediately searches Stack Overflow/LLM
- Copies the first answer that seems to work
- Doesn't understand why it works, just that it does
- Moves on to the next task

### **The Deep-Diving Engineer**
- Hits a problem → tries to understand it first
- Searches Stack Overflow/LLM for context, not just solutions
- Reads multiple answers/asks follow up questions to understand different approaches
- Checks the documentation to understand the underlying concepts
- Understands the problem in a way that they will never be flummoxed by it again

The difference isn't intelligence - it's curiosity and methodology.

## Beyond the fluff: The Documentation Deep Dive

One of my favorite interview question when I used to interview people who claimed they knew Django: *"What is the Request/Response cycle? How does a middleware work?"*

It's a fairly easy question but at best 1/15 engineers could answer it. How can you claim to know Django if you don't even know the basic lifecycle in it? How data flows in the framework?

The best engineers I know are **not afraid to jump into the documentation**. They understand that tutorials and blog posts show you one way to do something, but documentation shows you all the ways - and more importantly, the intended patterns and design philosophy. Each system has its own needs, its own requirements and you will not know how to truly code well till you understand the underlying principles and customize it to your needs.

## Going to the Source: Reading Library Code

This is where exceptional engineers separate themselves from the pack. When faced with a library that doesn't behave as expected, what's their first instinct?

### **Most Engineers:**
"This library doesn't have the functionality I need" or "This library is magic" - both indicate a lack of curiosity about how things actually work.

### **Good Engineers:**
"Let me see how this actually works" - and they dive into the source code.

I learned this habit out of necessity but boy I am glad I did. You must learn to read code. And reading other people's code - especially well-written library code - teaches you patterns and techniques you'd never discover otherwise.

**Anecdote:** I remember once I was unable to find out why some particular library was not working as expected and leaking memory. Out of desperation, I went into the source code of the library and put debug statements everywhere. Not only was I able to find the exact place where the memory was being leaked but I learnt so much about how good code is written. How functionality is abstracted at the level of a library.

## The First Reaction Test

Here's what I watch for when engineers encounter a non-obvious problem:

### **Option A: The Immediate Escalation**
- "I don't know how to do this"
- "Can someone help me?"
- "This is too complex"

### **Option B: The Investigation**
- "Let me understand what's happening here"
- "I wonder if this is related to X or Y"
- "Let me try to isolate the problem"
- "Let me collect some data before I ask for help"

Both approaches eventually get to a solution, but they create very different learning outcomes. Engineers who investigate first don't just solve the immediate problem - they build mental models that help them solve similar problems in the future. Even if they fail to solve the problem, any help they get will make much more sense to them because they can understand why a problem occurred and how the solution fits into the bigger picture.

## The Debugging Philosophy

Nothing reveals an engineer's depth like watching them debug. Here are the patterns I look for:

### **Systematic vs. Random**
- **Random:** Change things until something works
- **Systematic:** Form hypotheses, test them methodically, understand the results

### **Symptoms vs. Root Causes**
- **Symptoms:** "Let me just catch this exception and log it"
- **Root Causes:** "Let me understand why this exception is happening"

### **Local vs. Comprehensive**
- **Local:** "My code is fine, it must be the database/network/other team's fault"
- **Comprehensive:** "Let me trace this through the entire system to see where it breaks"

## Why Depth Matters More Than Breadth

In a field that changes as rapidly as software development, the ability to go deep is more valuable than any specific knowledge. Frameworks come and go, languages evolve, best practices shift - but the mindset of understanding systems deeply remains constant.

**The deep-diving engineer can:**
- Debug issues that would stump others
- Make informed decisions about trade-offs
- Adapt quickly to new technologies
- Build systems that others can understand and maintain

**The surface-level engineer:**
- Gets stuck when Stack Overflow doesn't have the answer
- Will not even understand if the LLM gives a wrong answer
- Makes cargo-cult decisions based on what they've seen work elsewhere
- Struggles with novel problems that don't fit known patterns
- Builds systems that work but are hard to maintain or extend

## Cultivating Depth

If you recognize yourself as more of a surface-level engineer, don't panic. Depth is a habit that can be developed:

### **Start with Documentation**
Before reaching for Stack Overflow/LLM, try the official docs. Yes, they're sometimes poorly written or incomplete but they're also the authoritative source of truth about how something is supposed to work. If that doesn't work, just dive into the source code.

### **Read Error Messages Carefully**
Error messages are not obstacles to be bypassed - they're clues to be investigated. What is the system trying to tell you? What assumptions did you make that turned out to be wrong?

### **Embrace the Source Code**
Modern development tools make it easy to jump to the definition of any function or class. Use this! Understanding how the tools you use actually work will make you a better engineer.

### **Ask "Why" Three Times**
When something doesn't work as expected, don't stop at making it work. Ask why it didn't work, why that caused a problem, and why the system is designed that way.

### **Teach Others**
Nothing forces you to understand something deeply like having to explain it to someone else. Write blog posts, answer questions, give talks. Teaching reveals the gaps in your own understanding.

## The Compound Effect of Depth

Engineers who go deep don't just solve problems faster - they are able to build the muscle to solve unique problems. They tackle challenges that would overwhelm others because they have the tools and mindset to understand complex systems.

More importantly, they become the engineers that others want to work with. They're the ones who can debug the mysterious production issue, who can evaluate whether a new technology is worth adopting, who can make architectural decisions with confidence.

## Looking for Depth in Others

When I'm interviewing or working with other engineers, I'm not looking for people who know everything. I'm looking for people who know how to figure things out.

- Do they ask good questions?
- Do they form hypotheses and test them?
- Are they curious about how things work under the hood?
- Do they read error messages and documentation?
- Can they explain complex concepts simply?

These traits are much better predictors of success than any specific technical knowledge.

---

## The Meta Question

As you're reading this, ask yourself: What's your first instinct when you encounter a problem you don't immediately know how to solve?

If it's to search for someone else's solution, that's fine - we all start there. But if you can develop the habit of understanding the problem first, of going to primary sources, of reading the code that's actually running - you'll become the kind of engineer that others rely on.

And in a field where the only constant is change, that depth of understanding is the skill that never becomes obsolete.

---

*The best engineers I've worked with aren't the ones who know the most - they're the ones who can learn the fastest. And learning fast requires going deep.* 