# grag
Guarded Retrieval Augmented Generation example

**Abstract**

**Problem**: Large Language Models (LLMs) are at the forefront of natural language processing advancements, thanks to their ability to understand and generate human-like text. However, challenges arise due to their tendency to occasionally produce irrelevant or misleading outputs and their inherent knowledge cutoff. This limitation means they might not be updated with the most recent information, necessitating the exploration of effective solutions beyond mere fine-tuning.

**Methodology**: Retrieval-augmented Generation (RAG) and its advanced iteration, Guarded Retrieval Augmented Generation (GRAG), were explored as potential solutions. RAG utilizes an intermediary approach, fetching relevant facts from external knowledge databases, grounding LLM outputs in verifiable data. Building on this, GRAG incorporates guardrails - specific controls that guide the model's outputs, such as circumventing politically charged topics or adhering to a set dialogue path. The methodology central to GRAG involves defining example queries or utterances and embedding them within a semantic vector space. This allows for rapid decision-making based on the semantic proximity of a user's query to predefined utterances.

**Conclusions**: The utilization of GRAG offers a more efficient and swifter alternative to the basic RAG method. It effectively mitigates the challenges of inaccurate or unrelated outputs from LLMs and ensures more precise and targeted outcomes.

**Relevance to practitioners and business**: As businesses integrate LLMs, GRAG offers means to ensure accuracy and relevance in AI outputs, catering to diverse business needs, from customer support to knowledge management.

## Installation

This project uses Conda for environment and package management. However, you are free to use your preferred method for installing packages if you are more comfortable with a different approach.

### Using Conda

If you choose to use Conda, here are the steps to set up the necessary environment for this project:

1. Ensure that Conda is installed on your system. Conda is an open-source package management and environment management system which runs on Windows, macOS, and Linux. If you do not have Conda installed, you can download it from [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (a minimal installer for Conda) or [Anaconda](https://www.anaconda.com/products/distribution) (which includes Conda and some additional tools).

2. Open your terminal (or Anaconda Prompt if you are on Windows) and navigate to the directory where the `environment.yml` file is located.

3. Create a new Conda environment and install all the required packages using the provided `environment.yml` file by running:

    ```bash
    conda env create -f environment.yml
    ```

4. Once the installation is complete, activate the new environment with:

    ```bash
    conda activate grag
    ```

For more information on managing Conda environments, please refer to the [official Conda documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).


## Running the Jupyter Notebook

After setting up the environment, you can run the Jupyter notebook `GRAG.ipynb` to execute the code:

1. Ensure that the Conda environment you created (or your custom environment) is activated.

2. Start Jupyter Notebook by running:

    ```bash
    jupyter notebook
    ```

3. In the Jupyter Notebook interface, navigate to the `GRAG.ipynb` file and open it.

4. Run the cells in the notebook as needed to execute the code.
