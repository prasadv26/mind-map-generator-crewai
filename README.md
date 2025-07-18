# mind-map-generator-crewai
Generate structured mind maps from raw text using CrewAI agents powered by LLMs. Converts articles or topics into concept hierarchies and renders them as JSON and images.

# 🧠 Mind Map Generator using CrewAI

This project transforms any raw idea or long-form article into a **visual mind map**, using a modular CrewAI agent system. It extracts key concepts, builds a concept hierarchy, outputs JSON, and renders an image using Graphviz.

---

## 🚀 Use Case

You want to summarize and visually organize long content (e.g., blog posts, articles, meeting notes, research papers) into a clear and structured **mind map**.

For example:

Input: A blog post on "Prompt Engineering"
→ Output: A mind map showing prompt types, methods, tools, and examples

yaml
Copy
Edit

This is ideal for:

- 👨‍🏫 Students learning complex topics  
- 🧑‍💼 Teams documenting workflows  
- 🧠 Brainstorming sessions  
- 🧾 Blog content visualization  

---

## 🧩 Architecture

+---------------------------+
| Input Topic or Text |
+------------+--------------+
|
v
+---------------------------+
| 🧠 Concept Extractor Agent |
+---------------------------+
|
v
+---------------------------+
| 🪜 Hierarchy Builder Agent |
+---------------------------+
|
v
+---------------------------+
| 🧾 JSON Formatter Agent |
+---------------------------+
|
v
+---------------------------+
| 🖼 Diagram Generator Agent |
| (Graphviz PNG renderer) |
+---------------------------+

yaml
Copy
Edit

---

## 📦 Output

- `mind_map_output.json` — Clean hierarchical concept structure  
- `mindmap.png` — Mind map image rendered from JSON

---

## 🛠 Tech Stack

- 🧠 [CrewAI](https://docs.crewai.com/)
- 🤖 OpenAI GPT-3.5-turbo via `LangChain`
- 📊 Graphviz for visualization
- 🐍 Python, Google Colab compatible

---

## ▶️ How to Run

1. Clone this repo
2. Open `mindmap_generator.ipynb` in Google Colab
3. Enter a topic or paste an article
4. Run all cells
5. View generated `mind_map_output.json` and `mindmap.png`

---

## 📌 Example Output

### Input:
> "Prompt engineering is the process of crafting inputs to get the best results from an LLM..."

### Output Image:

![Mindmap Image Example](mindmap.png)

---

## 📄 License

MIT License

