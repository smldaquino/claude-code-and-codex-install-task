# claude-code-and-codex-install-task
This repository documents the setup of two AI coding tools inside the Cursor IDE, the steps I completed, and the issues I ran into along the way.
 
## Tools Installed
- **Cursor IDE** — installed on my laptop running macOS 26.3.1
- **Claude Code** — installed and run via its CLI
- **OpenAI Codex** — installed and run via its CLI
  
## Steps Completed
1. Downloaded and installed Cursor from its website.
2. Installed Claude Code and authenticated with my Anthropic account.
3. Installed Codex and authenticated with my OpenAI account.
4. Created a GitHub account and a public repository.
5. Wrote this README describing the tools, steps, and issues.
6. Committed and pushed the changes to GitHub.

## Issues Encountered and How I Solved Them

### Couldn't find the Extensions view
After installing Cursor, I opened the application and searched for "Extensions" but could not find it in the View tab or anywhere else. I looked up the keyboard shortcut (`Cmd+Shift+X`), but it did not open the Extensions view either — it kept me on the default agent page. I then checked "Customize" in the left sidebar and searched the plugins for both Claude Code and Codex, but neither appeared.
 
### Installing Claude Code
Unable to find the tools through the marketplace, I asked Claude for help. While following its instructions, I accidentally ran the command `claude` in the agent view, which opened a chat session. From there, I was able to install Claude Code properly in the terminal using:
 
```bash
curl -fsSL https://claude.ai/install.sh | bash
```
 
I then logged into my Anthropic account and tested the tool in the terminal by asking Claude to say "Hello world!", which it did — confirming the installation was working.
 
### Installing Codex
 
Since I also couldn't find Codex in the application, I reasoned it could be installed the same way as Claude Code. I asked Claude to give me the command for installing Codex. I then installed the Codex CLI by running:
 
```bash
npm install -g @openai/codex
```
 
The first time I ran it, it opened an OpenAI login page, where I signed in with my account. After authenticating, Codex was ready to use. I tested it by asking it to say "Hello world!", which it did — confirming the installation was working.
 
### Creating the repository
 
Finally, I created a GitHub account and a public repository named [claude-code-and-codex-install-task](https://github.com/smldaquino/claude-code-and-codex-install-task/tree/main), ticking the "Add a README file" box, which is the file you are now reading.
 
