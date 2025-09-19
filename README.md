<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Multi-Source Search Agent Chatbot</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
      background-color: #f9f9f9;
      color: #333;
    }
    h1, h2, h3 {
      color: #222;
    }
    code {
      background: #eee;
      padding: 2px 5px;
      border-radius: 4px;
      font-size: 14px;
    }
    pre {
      background: #272822;
      color: #f8f8f2;
      padding: 12px;
      border-radius: 6px;
      overflow-x: auto;
    }
    .section {
      margin-bottom: 25px;
    }
    .box {
      background: #fff;
      border: 1px solid #ddd;
      border-radius: 6px;
      padding: 15px;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <h1>🧠 Multi-Source Search Agent Chatbot</h1>
  <p>
    A research-oriented chatbot powered by <b>OpenAI LLMs</b>, <b>LangGraph</b>, and <b>Bright Data</b> that fetches real-time information from 
    <b>Google</b>, <b>Bing</b>, and <b>Reddit</b>. It analyzes search results, synthesizes them, and provides a <b>final summarized answer</b>.
  </p>

  <div class="section">
    <h2>🚀 Features</h2>
    <ul>
      <li>🔍 Fetches results from <b>Google</b>, <b>Bing</b>, and <b>Reddit</b></li>
      <li>🧠 Uses <b>OpenAI GPT-4o</b> for analyzing and summarizing results</li>
      <li>🔗 Extracts and processes Reddit discussions</li>
      <li>📊 Orchestrates workflow using <b>LangGraph</b></li>
      <li>📝 Generates a final synthesized answer</li>
    </ul>
  </div>

  <div class="section">
    <h2>⚙️ Workflow</h2>
    <p>Here’s the flow of the LangGraph workflow:</p>
    <img src="workflow.png" alt="Workflow Diagram" width="600">
  </div>

  <div class="section">
    <h2>🛠️ Tech Stack</h2>
    <ul>
      <li>Python 3.10+</li>
      <li><a href="https://github.com/langchain-ai/langgraph">LangGraph</a></li>
      <li><a href="https://www.langchain.com/">LangChain</a></li>
      <li>OpenAI GPT-4o</li>
      <li>Bright Data SERP API</li>
      <li>Reddit API</li>
    </ul>
  </div>

  <div class="section">
    <h2>📂 Project Structure</h2>
    <pre>
.
├── main.py                # Main chatbot script
├── web_operations.py     # Google, Bing, Reddit fetch functions
├── prompts.py            # Prompt templates for analysis
├── .env                  # API keys
├── requirements.txt      # Dependencies
└── README.md             # Documentation
    </pre>
  </div>

  <div class="section">
    <h2>🔑 Setup & Installation</h2>
    <ol>
      <li><b>Clone the repository</b>
        <pre>git clone https://github.com/your-username/search-agent-chatbot.git
cd search-agent-chatbot</pre>
      </li>
      <li><b>Create virtual environment</b>
        <pre>python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows</pre>
      </li>
      <li><b>Install dependencies</b>
        <pre>pip install -r requirements.txt</pre>
      </li>
      <li><b>Set up <code>.env</code> file with your API keys</b>
        <pre>
OPENAI_API_KEY=your_openai_key
BRIGHT_DATA_API_KEY=your_bright_data_key
REDDIT_CLIENT_ID=your_reddit_client_id
REDDIT_CLIENT_SECRET=your_reddit_client_secret
        </pre>
      </li>
    </ol>
  </div>

  <div class="section">
    <h2>▶️ Usage</h2>
    <pre>python main.py</pre>
    <p><b>Example:</b></p>
    <pre>
Multi-Source Research Agent
Type 'exit' to quit

Ask me anything: What are the latest AI trends?

Final Answer:
AI trends include multimodal LLMs, edge AI, generative AI in healthcare, and synthetic data usage.
    </pre>
  </div>

  <div class="section">
    <h2>🎯 Purpose</h2>
    <p>
      This chatbot is designed to:
    </p>
    <ul>
      <li>Fetch <b>real-time</b> data across multiple sources</li>
      <li>Provide <b>comprehensive, fact-checked answers</b></li>
      <li>Combine <b>news</b> (Google, Bing) with <b>community insights</b> (Reddit)</li>
    </ul>
    <h3>Why use this?</h3>
    <ul>
      <li>✅ <b>Live search</b> → always up-to-date answers</li>
      <li>✅ <b>Multiple perspectives</b> → balanced and trustworthy</li>
      <li>✅ <b>Time-saving</b> → great for research & fact-checking</li>
    </ul>
  </div>
</body>
</html>
