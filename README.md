# Open source, open pipelines: Data ingestion with modern data stack 
### Presentation: [{ YOUR PRESENTATION NAME }](workshop/presentation_template.pdf)

## Workshop description
Data ingestion is the cornerstone of Data Engineering — it’s where every data journey begins. In this hands-on workshop, you’ll learn how to move data from anywhere to anywhere using the open-source modern data stack.

We’ll focus on practical skills, leveraging Python library dlt (data load tool) to ingest data from a REST API and load it into DuckDB, a fast and lightweight database. Whether you're just getting started with data pipelines or looking to modernize your current stack, this session will give you a solid foundation for building reliable, open-source ingestion workflows.

Come ready to write some code, get your hands dirty, and walk away with real-world ingestion superpowers.

## Requirements
* PyLadies Amsterdam uses [uv](https://docs.astral.sh/uv/) for dependency management
* Google account if you want to use [Google Colab](https://colab.research.google.com/)
 
## Usage
### with uv
Run the following code:
```bash
git clone <github-url-of-workshop-repo>
cd <name-of-repo>

# create and activate venv, install dependencies
uv sync
```
### with Google collab
1. Visit [Google Colab](https://colab.research.google.com/)
2. In the top left corner select "File" &#8594; "Open Notebook"
3. Under "GitHub", enter the URL of the repo of this workshop
4. Select one of the notebooks within the repo.
5. At the top of the notebook, add a Code cell and run the following code:
```bash
!git clone <github-url-of-workshop-repo>
%cd <name-of-repo>
!pip install -r requirements.txt
```
### for a workshop giver
To get started, open the `pyproject.toml` file and set the required Python version. The pre-selected version 3.8 is generally a safe choice for most use cases.

After you have specified the Python version, you can create a virtual environment with `uv venv` and add packages with `uv add <package>`. Before the workshop, you can generate a requirements.txt file, which is needed e.g. for running code in GoogleColab, by running `uv export > requirements.txt`.

## Video record
Re-watch [this YouTube stream](https://www.youtube.com/live/3XKjbKsHL4k)

## Credits
This workshop was set up by @pyladiesams and @VioletM


## Appendix
### Pre-Commit Hooks

To ensure our code looks beautiful, PyLadies uses pre-commit hooks. You can enable them by running `pre-commit install`. You may have to install `pre-commit` first, using `uv sync`, `uv pip install pre-commit` or `pip install pre-commit`.

Happy Coding :)
