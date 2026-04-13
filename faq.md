Answers to common frequently asked questions.

## What is Pocketenv?

Pocketenv is an open-source platform that lets you run **ephemeral development sandboxes in the cloud**. It allows you to quickly start isolated environments to run commands, test code, or execute AI agents without setting up infrastructure manually.

## Do I need to install anything to use Pocketenv?
No. Pocketenv environments run remotely. You can connect through the web interface or the CLI without installing heavy dependencies locally.

## What runtimes does Pocketenv support?
Pocketenv supports multiple sandbox runtimes depending on your needs, including:
- Daytona
- Deno Sandbox
- Vercel Sandbox
- Cloudflare Sandbox
- Sprite
- Modal
- Runloop
- E2B

You can choose the runtime that best fits your workflow.

## What can I run inside a sandbox?
You can run almost anything typically used in development environments, such as:
- CLI tools
- AI coding agents
- compilers and build tools
- scripts
- development servers

Many base templates already include tools like **git, nix, mise, docker, or pkgx.**

## Are sandboxes persistent?
By default, Pocketenv sandboxes are ephemeral.
This means the environment can be destroyed after use.

However, you can persist data using:
- Volumes
- Files
- Environment variables
- Secrets

## Can I securely store secrets?
Yes. Pocketenv supports **encrypted Secrets** that can be injected into sandboxes as environment variables.

This allows you to safely store API keys, tokens, or credentials.

## Can I access my sandbox through SSH?
Yes. Pocketenv allows you to attach **SSH keys** to your environment so you can connect securely.

## Can I mount files or volumes?
Yes. Pocketenv supports:
- Files → injected into the sandbox filesystem
- Volumes → persistent storage shared across sessions

## Is Pocketenv open source?
Yes. Pocketenv is fully open source.

You can find the project here:
https://github.com/pocketenv-io/pocketenv


## Is Pocketenv ready for production?
Pocketenv is currently evolving quickly. While it is already usable, some features may still be experimental.

Feedback and contributions are welcome.
