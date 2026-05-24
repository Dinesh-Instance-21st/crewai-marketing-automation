# CrewAI Marketing Automation

An AI-powered marketing strategy automation system built with **CrewAI**, designed to streamline content creation, marketing strategy development, and campaign management using autonomous AI agents.

## 🤖 Features

- **AI-Powered Marketing Agents**: Autonomous agents handle different marketing roles
- **Content Creation**: Automatically generate marketing content (blog posts, social media posts, etc.)
- **Strategy Development**: Create comprehensive marketing strategies based on market research
- **Web Research**: Real-time web scraping and search capabilities using Serper and web scraping tools
- **Multi-Agent Collaboration**: Agents work together with delegation capabilities
- **Google Gemini Integration**: Leverages Google's Gemini 3.5 Flash model for intelligent responses

## 🛠 Tech Stack

- **CrewAI**: Multi-agent AI framework
- **Google Gemini 3.5 Flash**: LLM backbone
- **CrewAI Tools**: Serper, Web Scraping, File I/O operations
- **Python 3.13+**: Programming language
- **UV**: Fast Python package installer

## 📋 Prerequisites

- Python 3.13 or higher
- Google API Key (for Gemini)
- Serper API Key (for web search)

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/Dinesh-Instance-21st/crewai-marketing-automation.git
cd crewai-marketing-automation
```

### 2. Set Up Environment

Create a `.env` file in the root directory with:

```env
GOOGLE_API_KEY=your_google_api_key_here
SERPER_API_KEY=your_serper_api_key_here
```

### 3. Install Dependencies

```bash
# Using UV (recommended)
uv sync

# Or using pip
pip install -r requirements.txt
```

### 4. Activate Virtual Environment

```bash
# On Windows
.venv\Scripts\Activate.ps1

# On macOS/Linux
source .venv/bin/activate
```

### 5. Run the Project

```bash
python main.py
```

## 📁 Project Structure

```
crew_ai/
├── main.py                          # Entry point
├── marketing-crew/
│   ├── crew.py                     # Crew configuration and agent definitions
│   └── config/
│       ├── agents.yaml             # Agent configurations
│       └── tasks.yaml              # Task definitions
├── resources/
│   └── drafts/                     # Generated content storage
│       ├── marketing_strategy.md
│       ├── blogs/
│       └── posts/
├── pyproject.toml                  # Project metadata
├── requirements.txt                # Python dependencies
├── .env                            # Environment variables (not committed)
├── .gitignore                      # Git ignore rules
└── README.md                       # This file
```

## 🤝 Marketing Crew Agents

The crew includes the following agent roles:

- **Head of Marketing**: Leads strategy development and content planning
- **Content Creator**: Generates marketing content across channels
- **Social Media Manager**: Manages social media strategy and posts
- And more specialized marketing agents...

## 📝 Configuration

### agents.yaml
Define agent roles, goals, and backstories in `marketing-crew/config/agents.yaml`

### tasks.yaml
Define tasks for each agent in `marketing-crew/config/tasks.yaml`

## 🔧 Customization

Modify the following to customize your marketing automation:

1. **Agent Roles**: Edit `marketing-crew/config/agents.yaml`
2. **Tasks**: Edit `marketing-crew/config/tasks.yaml`
3. **LLM Settings**: Adjust temperature and model in `marketing-crew/crew.py`
4. **Tools**: Add/remove tools from agent configurations

## 🐛 Troubleshooting

### API Key Issues
- Ensure `GOOGLE_API_KEY` and `SERPER_API_KEY` are set in `.env`
- Check that keys have proper permissions

### Module Not Found
```bash
# Reinstall dependencies
pip install -r requirements.txt
```

### Virtual Environment Issues
```bash
# Recreate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1  # Windows
source .venv/bin/activate   # macOS/Linux
pip install -r requirements.txt
```

## 📚 Resources

- [CrewAI Documentation](https://docs.crewai.com/)
- [Google Gemini API](https://ai.google.dev/)
- [Serper API Documentation](https://serper.dev/)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or support, please open an issue on GitHub.

---

**Built with ❤️ using CrewAI**
