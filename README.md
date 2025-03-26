# LangGraph Visualisation Tool

A tool for visualising and understanding LangGraph execution flows using Mermaid and PNG formats.

## Overview

This project provides a visualization tool for LangGraph applications, allowing developers to better understand and debug their agent workflows. It supports both Mermaid diagram generation and PNG exports, making it easy to integrate into documentation or presentations.

## Features

- 🔄 Mermaid.js diagram generation
- 📊 PNG export support
- 🎨 Multiple visualisation options
- 🛠️ Easy integration with existing LangGraph applications
- 📱 Support for different output formats

## Tech Stack

- **Python 3.x**
- **LangChain** - Framework for building context-aware reasoning applications
- **LangGraph** - Framework for building resilient language agents as graphs
- **Jupyter Notebook** - Interactive computing environment (Optional)
- **Graphviz** - Graph visualisation software
- **Pygraphviz** - Python interface to Graphviz
- **Mermaid.js** - JavaScript based diagramming and charting tool

## Installation

1. Clone the repository:
```bash
git clone https://github.com/pakagronglb/langgraph-visualisation-tool.git
cd langgraph-visualisation-tool
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Install Graphviz (required for PNG generation):
```bash
# macOS
brew install graphviz

# Ubuntu/Debian
sudo apt-get install graphviz graphviz-dev

# Windows
choco install graphviz
```

## Usage

1. Import the necessary modules in your Jupyter notebook:
```python
from IPython.display import Image, display
```

2. Generate visualizations:
```python
# For Mermaid diagram
print(app.get_graph().draw_mermaid())

# For PNG output
display(Image(app.get_graph().draw_png()))
```

## Examples

The repository includes example notebooks demonstrating:
- Basic graph visualisation
- Custom styling and formatting
- Different output formats
- Integration with existing LangGraph applications

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Credits

This project builds upon the excellent work of:
- [LangChain](https://github.com/langchain-ai/langchain) - 🦜🔗 Build context-aware reasoning applications
- [LangGraph](https://github.com/langchain-ai/langgraph) - Build resilient language agents as graphs

Special thanks to the [@langchain-ai](https://github.com/langchain-ai) team for providing the foundational frameworks that make this tool possible.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
