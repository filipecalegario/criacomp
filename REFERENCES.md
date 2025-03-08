# Organized References 

## Ideas to be implemented

* Use Claude 3.7 to create charts based on an input screenshot for a chart for inspiration and paste in the data

## Tools to be tested

* [Postman AI Agent Builder | Postman API Network](https://www.postman.com/ai-on-postman/postman-ai-agent-builder/overview)
* [Stanford Storm](https://storm.genie.stanford.edu/)
* [Chunkr | Open Source Document Intelligence API](https://chunkr.ai/): API service to convert complex documents into LLM/RAG-ready chunks
* [Mistral OCR | Mistral AI](https://mistral.ai/en/news/mistral-ocr): Introducing the world’s best document understanding API
* [Hello FastHTML and MonsterUI - Drew Echerd's Blog](https://www.drewecherd.com/post/hello-fasthtml-monsterui): a powerful combination for building modern web applications in Python
* [Poe](https://poe.com/)
* [CopyCoder](https://copycoder.ai/): Upload images of full applications, UI mockups, or custom designs and use our generated prompts to build your apps faster.
* [Manus](https://manus.im/): Manus is a general AI agent that bridges minds and actions: it doesn't just think, it delivers results.

## Videos to be watched

* [How I use LLMs - YouTube](https://www.youtube.com/watch?v=EWvNQjAaOHw&t=475s): Andrej Karpathy
* [How to build & deploy agents, according to OpenAI - YouTube](https://www.youtube.com/watch?v=joHR2pmxDQE): AI Engineer Summit

## Papers to be read

## Posts to be read

* [Anthropic’s Recommendations to OSTP for the U.S. AI Action Plan \ Anthropic](https://www.anthropic.com/news/anthropic-s-recommendations-ostp-u-s-ai-action-plan)
* [Opinion | The Government Knows A.G.I. Is Coming - The New York Times](https://archive.ph/UGfvQ#selection-1419.8-1419.68): an edited transcript of an episode of “The Ezra Klein Show.”

## Courses to be taken

* [The Hugging Face Agents Course](https://huggingface.co/agents-course)
* [The Reasoning Course - Hugging Face NLP Course](https://huggingface.co/learn/nlp-course/en/chapter12/1?fw=pt)
* [microsoft/generative-ai-for-beginners](https://github.com/microsoft/generative-ai-for-beginners): 21 Lessons, Get Started Building with Generative AI 🔗 https://microsoft.github.io/generative-ai-for-beginners/
* [CSE 291 - AI Agents - UCSD CSE](https://pearls-lab.github.io/ai-agents-course/index.html)

## Catalog for more references (branching factor)

* [panaversity/learn-agentic-ai](https://github.com/panaversity/learn-agentic-ai): Learn Agentic AI using CrewAI, LangChain, LangGraph, and Knowledge Graphs.
* [LLM apps built with RAG and AI agents / X](https://x.com/victor_explore/status/1896374933003153668): A curated collection of awesome LLM apps built with RAG and AI agents
* [patchy631/ai-engineering-hub](https://github.com/patchy631/ai-engineering-hub/tree/main)

## Tested Tools

* [microsoft/TinyTroupe: LLM-powered multiagent persona simulation for imagination enhancement and business insights](https://github.com/microsoft/TinyTroupe): defining characters and simulating their interaction
* [UVR5 UI - a Hugging Face Space by TheStinger](https://huggingface.co/spaces/TheStinger/UVR5_UI): music source separation with multiple models. A good one to separate voice BS-Roformer-Viperx-1296
* [Di♪♪Rhythm - a Hugging Face Space by ASLP-lab](https://huggingface.co/spaces/ASLP-lab/DiffRhythm): input lyrics with timestamps. English-only.

# Thematic References

## MCP Hype

* [Matt Wolfe on X: "MCPs (Model Context Protocols) are the AI buzzword of the moment. If you’re into “vibe coding” or want to connect your Claude to external tools, this is a pretty big unlock. I found this thread about them valuable…" / X](https://x.com/mreflow/status/1897317957539389593)
* [Santiago on X: "Anthropic's MCP is a thing of beauty. This makes AI agents 100x more powerful. MCP stands for "Model Context Protocol." It's an open standard for connecting AI with data. Instead of worrying about 10,000 different ways to do the same thing, MCP provides a standard approach. •" / X](https://x.com/svpino/status/1896991534421307570)
* [Alex Volkov (Thursd/AI) on X: "ok I'm MCP pilled, who's been using them for a while now? Who's written their own? Who do I need to follow to help me prepare for @thursdai_pod talking about MCPs? https://t.co/Ai7fOi19Ar" / X](https://x.com/altryne/status/1897051777352294424)
* [will brown on X: "claude is building his own MCP tool setup in public https://t.co/Ug8pnD31j7" / X](https://x.com/willccbb/status/1896778724194062830)
* [jason liu (NY 2/18-3/3) on X: "MCP vs OpenAPI https://t.co/eJBGLhSovE" / X](https://x.com/jxnlco/status/1897338699672859094)

### MCP Deep Investigation

* [Introducing the Model Context Protocol \ Anthropic](https://www.anthropic.com/news/model-context-protocol)
  * an open standard that enables developers to build secure, two-way connections between their data sources and AI-powered tools.
  * developers can either expose their data through MCP servers or build AI applications (MCP clients) that connect to these servers.
* [Model Context Protocol](https://github.com/modelcontextprotocol): Model Context Protocol (MCP) is an open protocol that enables seamless integration between LLM applications and external data sources and tools.
* [Introduction - Model Context Protocol](https://modelcontextprotocol.io/introduction)
  * Think of MCP like a USB-C port for AI applications.
  * MCP helps you build agents and complex workflows on top of LLMs.
* Examples
  * [Example Servers - Model Context Protocol](https://modelcontextprotocol.io/examples)
  * [abhiz123/todoist-mcp-server](https://github.com/abhiz123/todoist-mcp-server/tree/main): MCP server for Todoist integration enabling natural language task management with Claude
* List of Servers
  * [modelcontextprotocol/servers: Model Context Protocol Servers](https://github.com/modelcontextprotocol/servers)
  * [Awesome MCP Servers](https://mcpservers.org/)
  * [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers): A collection of MCP servers.
  * [Composio MCP Server](https://mcp.composio.dev/): Connect Cursor, Windsurf, and Claude to 100+ fully managed MCP Servers with built-in auth
    * These servers are built by the community and are hosted by Composio
* [Example Clients - Model Context Protocol](https://modelcontextprotocol.io/clients)
  * Resources, prompts, and tools
* [Building MCP with LLMs - Model Context Protocol](https://modelcontextprotocol.io/tutorials/building-mcp-with-llms)
  * Attention for the use of llms-full.txt pattern!
* [https://t.co/t3tTSTr02y" / X](https://x.com/mckaywrigley/status/1898109392341385509)
  * Now more often local servers. In the future, hosted servers and auth.
* Add Supabase to Cursor via MCP
  * [https://t.co/aQITshj3Er" / X](https://x.com/dshukertjr/status/1896531501514109056)

## Cursor MDC Rules Deep Investigation

* [bmadcode/cursor-auto-rules-agile-workflow](https://github.com/bmadcode/cursor-auto-rules-agile-workflow/tree/main): Cursor Automatic Rules Generation with Agile Cursor Workflow Template
  
## About Embeddings

* [(416) The Hidden Life of Embeddings: Linus Lee - YouTube](https://www.youtube.com/watch?v=YvobVu1l7GI)
* [thesephist/contra-bottleneck-t5-large-wikipedia · Hugging Face](https://huggingface.co/thesephist/contra-bottleneck-t5-large-wikipedia): able to encode text up to 512 tokens into an embedding, then reconstruct the original text from the embedding
* [If you're not fine-tuning and embedding models, you're Blockbuster, not Netflix.](https://x.com/jxnlco/status/1897337783058133080): [Video about Embedding Models Fine-tuning](https://maven.com/p/1ea9c9/glean-s-embedding-model-for-enterprise-adapted-ai)

## Ideas for CRIACOMP groups

* [Blog/articles/multi_agents.md at main · YukoOshima/Blog](https://github.com/YukoOshima/Blog/blob/main/articles/multi_agents.md): a multi-agent setup for generating and validating flash cards.

## FOR FURTHER ANALYSIS

* [The /llms.txt file – llms-txt](https://llmstxt.org/): o que é esse padrão?
* [(2) Adam Sardo on X: "// .cursor/rules/plan.mdc When asked to enter "Planner Mode" deeply reflect upon the changes being asked and analyze existing code to map the full scope of changes needed. Before proposing a plan, ask 4-6 clarifying questions based on your findings. Once answered, draft a" / X](https://x.com/sardo_adam/status/1896269828509536658)
* [Kyle Corbitt on X: "🕵️ Can smaller, open-weight models match state-of-the-art reasoning performance? We investigated using GRPO on "Temporal Clue," surpassing R1, o1, and o3-mini—and nearly matching Sonnet 3.7 at over 100x lower inference cost. Here's how: 👇 (1/6) https://t.co/odV85JMaic" / X](https://x.com/corbtt/status/1897735437340627405)
* [Kirk Borne on X: "Source: @ordax on LinkedIn &gt;&gt; 10 YouTube channels for learning AI: 🎓 1) Andrej Karpathy – Deep yet accessible lectures on deep learning, LLMs, and an intro course on neural networks. https://t.co/DjCX8Va4tt 📊 2) 3Blue1Brown – Stunning visualizations that make abstract https://t.co/6b8yw09WNL" / X](https://x.com/KirkDBorne/status/1897510190267646307): pegar os usuários do Twitter deles
