# DSA2101 Project -- UN Voting Patterns (Data Visualisation)

## Research Motivation 
As an organisation, the United Nations (UN) aims to maintain international peace and security, foster friendly relations among nations, and promote cooperation in solving global challenges. However, the effectiveness of the UN remains mixed. While it has been instrumental in raising global challenges, its role as a neutral decision-making platform has been shaped by the differing interests and influence of its member states. Particularly, the Cold War (1947–1991) marked one of the most pivotal periods for the UN. As global politics became defined by ideological confrontation between the United States (US) and the Soviet Union (USSR), many countries found themselves situated within an intensely polarised UN. This period also saw the emergence of newly independent states from decolonisation, whose votes introduced new dynamics and shifted the balance of global influence. Hence, each member state’s vote reflected broader considerations on strategic alignments and alliances within a bipolar world order. 

This leads us to the key research question of this project – <u>how did patterns of geopolitical alignment evolve during the Cold War as reflected by the voting dynamics in the UN General Assembly (UNGA)?</u> To explore this in greater detail, this project examines how patterns of geopolitical alignment evolved in UNGA voting during the Cold War, through analysing the UN Votes dataset and implementing visualisations that illustrate (1) **change in global interest on various issues** (colonialism, economic development, etc.), (2) **each country’s alignment with the United States and the Soviet Union**, and (3) **different countries’ alignment with the majority vote for each issue**. Through these visualisations, we aim to trace not only how the Cold War shaped UN decision-making, but also how smaller nations navigated between competing spheres of influence. 

## Key Findings
Our report details 3 key findings: 
(1) Arms Control and Disarmament (di) and Nuclear Weapons & Materials (nu), once issues that garnered little prominence in UN resolutions, steadily gained international interest as the cold war progressed. This is evidenced by the proportion of resolutions each year devoted to these two issues. 

(2) 3 voting blocs are evident: The Western bloc that showed strong alignment with the US (Canada, Western Europe, Japan, Australia, and South Africa), The Eastern Bloc that showed strong alignment with the USSR, and members of the Non-Aligned Movement (NAM) that sought to remain outside of the Cold War binary. This closely, if not identically, resembles the "First World, Second World, Third World" political framing that still defines nation-states today. 

(3) Majority consensus was shaped by the Non-Aligned Movement, which contained the highest number of nation-states in its voting bloc. Nonetheless, the data continues to paint a picture of a (powerful) Western bloc, small in number, that often acts in opposition to the majority viewpoint. 

Taken together, our analyses reveal that voting dynamics in the UN General Assembly during the Cold War mirrored the broader geopolitical landscape of the era, while the growing participation of post-colonial states introduced a more multipolar and independent dimension to the "US-USSR" binary. 

## Running the Notebook

The analysis is contained in [`dsaprojectFINAL.ipynb`](dsaprojectFINAL.ipynb). It
downloads the UN voting data from the TidyTuesday GitHub repository when it
runs, so an internet connection is required.

### Prerequisites

- Python 3.11 or later
- `pip`

### Setup and run

From the project directory, create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the project dependencies, plus the notebook and plotting packages used
by the analysis:

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt seaborn jupyterlab
```

Start JupyterLab:

```bash
jupyter lab
```

In the browser window that opens, select `dsaprojectFINAL.ipynb` and choose
**Run > Run All Cells**. The first cells download and prepare the data; the
remaining cells generate the static charts and interactive Plotly
visualisations.

To run it from VS Code instead, open the project folder, select the `.venv`
Python interpreter, open `dsaprojectFINAL.ipynb`, and use **Run All**.

### Troubleshooting

- If a data-loading cell fails, verify that you are online and that GitHub is
  reachable; the notebook reads the CSV files from GitHub rather than from a
  local `data/` directory.
- If Plotly figures do not appear, rerun the first setup/import cell before
  running the visualisation cells.
- When finished, leave the virtual environment with `deactivate`.

