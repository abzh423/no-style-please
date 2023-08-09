---
layout: post
category: piston
---

So I had to implement configuration files for piston and was wondering about what to choose.
There were some options available and I started considering the drawbacks and advantages of each.
Here are the technologies assessed:
- Yaml
- Toml
- Json

## Yaml
Yaml is a human-friendly data serialization language for all programming languages. 
Given that definition we can infer it's easy to read, quite obvious right?
Yaml is also quite challenging to parse because of how much flexibility with types it offers;
not to mention the security vulnerabilities that cmay be introduced due to that.

## Json
Challenging to read, simple structure for types of which there are six. And nice to parse.
It's a good choice if humans don't touch the data being structured with Json.
For example, created by the machine and parsed by the machine. No human involvment.

## Toml
Toml is like Yaml easy to read for humans, but it has simple system for types and doesn't tend to be unsafe.
Toml is human friendly and at the same time machine friendly (easier to parse than Yaml), aims to take the golden middle to say.

## What did I choose?
So I went with Toml, we needed configuration files for users to change the settings of software.
