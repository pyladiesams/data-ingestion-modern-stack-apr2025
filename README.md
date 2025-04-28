# Open source, open pipelines: Data ingestion with modern data stack 

## Workshop description
Data ingestion is the cornerstone of Data Engineering — it’s where every data journey begins. In this hands-on workshop, you’ll learn how to move data from anywhere to anywhere using the open-source modern data stack.

We’ll focus on practical skills, leveraging Python library dlt (data load tool) to ingest data from a REST API and load it into DuckDB, a fast and lightweight database. Whether you're just getting started with data pipelines or looking to modernize your current stack, this session will give you a solid foundation for building reliable, open-source ingestion workflows.

Come ready to write some code, get your hands dirty, and walk away with real-world ingestion superpowers.

## Requirements
* PyLadies Amsterdam uses [uv](https://docs.astral.sh/uv/) for dependency management
* Google account if you want to use [Google Colab](https://colab.research.google.com/)
 
## Usage

There are two ways of running this workshop:

1. With Google Colab (recommended)
2. On local instance of Jupyter Notebook

### with Google Colab

You can open direct links to Colab:
* [Workshop](https://drive.google.com/file/d/19vJvOPtWV9CHsTyKIjtPNWcDjy5LafcE/view?usp=sharing)
* [Solutions](https://colab.research.google.com/drive/1-d4l17qbeKPq3NLEkS0P20577M5EMDRR?usp=sharing)

Or you can add `.ipynb` from this repository to your Google Drive the following way:

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

### on local Jupyter Notebook (with uv)

Run the following code:
```bash
git clone <github-url-of-workshop-repo>
cd <name-of-repo>

# create and activate venv, install dependencies
uv sync
```

And start the Jupyter Notebook:

```bash
uv run jupyter notebook
```

## Video record
Re-watch [this YouTube stream](https://www.youtube.com/live/3XKjbKsHL4k)

## Credits
This workshop was set up by @pyladiesams and @VioletM


## Appendix
### Pre-Commit Hooks

To ensure our code looks beautiful, PyLadies uses pre-commit hooks. You can enable them by running `pre-commit install`. You may have to install `pre-commit` first, using `uv sync`, `uv pip install pre-commit` or `pip install pre-commit`.

Happy Coding :)
