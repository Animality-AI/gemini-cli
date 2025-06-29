
<div align="center">

```
 █████╗ ███╗   ██╗██╗███╗   ███╗ █████╗ ██╗     ██╗████████╗██╗   ██╗     █████╗ ██╗
██╔══██╗████╗  ██║██║████╗ ████║██╔══██╗██║     ██║╚══██╔══╝╚██╗ ██╔╝    ██╔══██╗██║
███████║██╔██╗ ██║██║██╔████╔██║███████║██║     ██║   ██║    ╚████╔╝     ███████║██║
██╔══██║██║╚██╗██║██║██║╚██╔╝██║██╔══██║██║     ██║   ██║     ╚██╔╝      ██╔══██║██║
██║  ██║██║ ╚████║██║██║ ╚═╝ ██║██║  ██║███████╗██║   ██║      ██║    ██╗██║  ██║██║
╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝╚═╝     ╚═╝╚═╝  ╚═╝╚══════╝╚═╝   ╚═╝      ╚═╝    ╚═╝╚═╝  ╚═╝╚═╝
```// Modified by Animality AI, 2025-06-29
# animality.ai CLI

This CLI is an Apache-2.0 derivative of Google's Gemini CLI. LICENSE & NOTICE preserved.

This repository contains the animality.ai CLI, a command-line AI workflow tool that connects to your
tools, understands your code and accelerates your workflows.

With the animality.ai CLI you can:

- Query and edit large codebases in and beyond the AI model's 1M token context window.
- Generate new apps from PDFs or sketches, using multimodal AI capabilities.
- Automate operational tasks, like querying pull requests or handling complex rebases.
- Use tools and MCP servers to connect new capabilities, including [media generation with Imagen,
  Veo or Lyria](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/tree/main/experiments/mcp-genmedia)
- Ground your queries with the [Google Search](https://ai.google.dev/gemini-api/docs/grounding)
  tool, built in to the AI model.


</div>

---


   ```bash
   npx @animality/cli
   ```


The Gemini CLI is your **intelligent development assistant** that bridges the gap between natural language and code execution. Think of it as having a senior developer who understands your entire codebase, can read your mind, and executes complex tasks with surgical precision.


   ```bash
   npm install -g @animality/cli
   animality-cli
   ```

3. **Pick a color theme**
4. **Authenticate:** When prompted, sign in with your personal Google account. This will grant you up to 60 model requests per minute and 1,000 model requests per day using the AI model.

You are now ready to use the animality.ai CLI!


---

### 🔑 Advanced Authentication

Need higher limits or specific models? Use an API key:

1. **Generate key**: Visit [Google AI Studio](https://aistudio.google.com/apikey)
2. **Set environment variable**:
   ```bash

   export GEMINI_API_KEY="your_key_here"

   ```
3. **Enterprise setup**: See [authentication guide](./docs/cli/authentication.md) for Google Workspace accounts

## 📚 Examples


Once the CLI is running, you can start interacting with AI from your shell.


### 🆕 Starting Fresh
```bash
mkdir my-awesome-project && cd my-awesome-project
gemini
```
```text
> Write me a Discord bot that answers questions using a FAQ.md file I will provide
```


```sh
cd new-project/
animality-cli
> Write me a Discord bot that answers questions using a FAQ.md file I will provide
```

### 🚀 Real-World Examples


```sh
git clone https://github.com/animality-ai/cli
cd cli
animality-cli
> Give me a summary of all of the changes that went in yesterday

</details>

<details>
<summary><b>🛠️ Feature Development</b></summary>

```text
> Implement a first draft for GitHub issue #123

> Help me migrate this codebase to the latest version of Java. Start with a plan

> Add TypeScript support to this project with proper configuration
```
</details>

<details>
<summary><b>🤖 Automation & Workflows</b></summary>

```text
> Make me a slide deck showing the git history from the last 7 days, grouped by feature

> Create a full-screen web app for displaying our most active GitHub issues

> Set up a CI/CD pipeline that deploys to staging on every PR
```
</details>


Start by `cd`ing into an existing or newly-cloned repository and running `animality-cli`.


```text
> Convert all images in this directory to PNG and rename them using EXIF dates

> Organize my PDF invoices by month of expenditure

> Clean up this messy JavaScript project and add proper linting
```
</details>

---

### 📖 Next Steps

| Resource | Description |
|----------|-------------|
| [🚀 CLI Commands](./docs/cli/commands.md) | Master all available commands |
| [🔧 Troubleshooting](./docs/troubleshooting.md) | Solve common issues quickly |
| [📚 Full Documentation](./docs/index.md) | Comprehensive guides |
| [🤝 Contributing](./CONTRIBUTING.md) | Help improve Gemini CLI |
| [💡 Popular Tasks](#-popular-use-cases) | Get inspired with real examples |

## 🌟 Popular Use Cases

### 🕵️ Code Exploration & Understanding
*Perfect for new team members or exploring unfamiliar codebases*

```bash
cd any-project && gemini
```

<table>
<tr>
<td width="50%">

**🔍 Architecture Deep Dive**
```text
> Describe the main pieces of this 
  system's architecture

> What are the key design patterns used?

> Show me the data flow from API 
  to database
```

</td>
<td width="50%">

**🔒 Security & Quality Review**
```text
> What security mechanisms are in place?

> Find potential vulnerabilities in 
  this authentication code

> Review this code for performance 
  bottlenecks
```

</td>
</tr>
</table>

### 🚀 Development & Feature Building
*From idea to implementation in minutes*

<table>
<tr>
<td width="50%">

**⚡ Rapid Prototyping**
```text
> Implement a first draft for 
  GitHub issue #123

> Create a REST API for user 
  management with authentication

> Build a React component for 
  file uploads with progress bars
```

</td>
<td width="50%">

**🔄 Migration & Modernization**
```text
> Migrate this codebase to 
  TypeScript with proper types

> Upgrade this React app from 
  class components to hooks

> Convert these REST endpoints 
  to GraphQL
```

</td>
</tr>
</table>

### 🤖 Automation & DevOps
*Let AI handle the repetitive tasks*

<table>
<tr>
<td width="50%">

**📊 Reporting & Analytics**
```text
> Create a dashboard showing git 
  activity by team member

> Generate a performance report 
  from these log files

> Build a monitoring dashboard 
  for system health
```

</td>
<td width="50%">

**🔧 Infrastructure & CI/CD**
```text
> Set up GitHub Actions for 
  automated testing and deployment

> Create Docker configuration 
  for this application

> Build a monitoring script for 
  server uptime
```

</td>
</tr>
</table>

### 🗂️ File & Data Management
*Organize and transform your data intelligently*

<table>
<tr>
<td width="50%">

**🖼️ Media Processing**
```text
> Convert all images to WebP format 
  and optimize for web

> Extract metadata from all photos 
  and organize by date

> Resize images for different 
  device breakpoints
```

</td>
<td width="50%">

**📄 Document Management**
```text
> Organize PDF invoices by 
  month and vendor

> Extract data from CSV files 
  and create summary reports

> Convert markdown docs to 
  structured JSON
```

</td>
</tr>
</table>

---

> 💡 **The key to success**: Be specific about what you want, provide context, and don't be afraid to iterate!

---

## 📋 Additional Resources

<div align="center">

### 🤝 Community & Support

[![GitHub Issues](https://img.shields.io/github/issues/google-gemini/gemini-cli.svg)](https://github.com/google-gemini/gemini-cli/issues)
[![GitHub Stars](https://img.shields.io/github/stars/google-gemini/gemini-cli.svg)](https://github.com/google-gemini/gemini-cli/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/google-gemini/gemini-cli.svg)](https://github.com/google-gemini/gemini-cli/network)

[💬 Discussions](https://github.com/google-gemini/gemini-cli/discussions) • [🐛 Report Bug](https://github.com/google-gemini/gemini-cli/issues/new) • [💡 Request Feature](https://github.com/google-gemini/gemini-cli/issues/new)

</div>

### 📚 Learning Resources

| Resource | Description |
|----------|-------------|
| [🎓 Tutorials](./docs/cli/tutorials.md) | Step-by-step guides for common tasks |
| [⚙️ Configuration](./docs/cli/configuration.md) | Customize Gemini CLI to your workflow |
| [🎨 Themes](./docs/cli/themes.md) | Beautiful color schemes for your terminal |
| [🔧 Advanced Features](./docs/cli/commands.md) | Power user commands and options |

### 🔗 Integrations

| Integration | Description |
|-------------|-------------|
| [🔌 MCP Servers](./docs/tools/mcp-server.md) | Connect external tools and services |
| [🌐 Web Search](./docs/tools/web-search.md) | Real-time information with Google Search |
| [📁 File System](./docs/tools/file-system.md) | Advanced file and directory operations |
| [💾 Memory](./docs/tools/memory.md) | Persistent context across sessions |

---

## ⚖️ Terms of Service and Privacy Notice


For details on the terms of service and privacy notice applicable to your use of Gemini CLI, see the [Terms of Service and Privacy Notice](./docs/tos-privacy.md).

---

<div align="center">

**Made with ❤️ by the Google Gemini team Modified with ☕️ by the Animality.ai Team**

*Transforming the way developers build, one command at a time.*

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

</div>

