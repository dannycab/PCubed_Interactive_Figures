# PCubed Interactive Figures

Snappy, self‑contained physics visuals you can open in any browser. Each HTML file is an interactive Plotly figure illustrating core mechanics concepts (constant acceleration, constant velocity, sinusoidal motion, and net force relationships). No server. No build. Just open and explore.

## Quick Peek
Directory `interactive/mechanics/` contains ready-to-open figures:

| Figure | Concept |
|--------|---------|
| `CA_position_vs_time.html` | Constant acceleration: position vs time |
| `CA_velocity_vs_time.html` | Constant acceleration: velocity vs time |
| `CA_velocity_vs_time_area_fill.html` | Velocity graph with area (displacement) shading |
| `CV_position_vs_time.html` | Constant velocity: position vs time |
| `CV_velocity_vs_time.html` | Constant velocity: velocity vs time |
| `CV_velocity_vs_time_area_fill.html` | Constant velocity with displacement area |
| `net_force_vs_position_discrete.html` | Discrete net force vs position samples |
| `net_force_vs_time_discrete.html` | Discrete net force vs time samples |
| `net_force_vs_time_smooth.html` | Smoothed net force vs time curve |
| `sinusoidal_position_vs_time_coarse_fine.html` | Comparing coarse vs fine sinusoidal sampling |

## Open a Figure (macOS)
Double‑click an HTML file OR from the project root:

```fish
open interactive/mechanics/CA_position_vs_time.html
```

## Regenerate / Modify Figures
The notebook `pcubed_plotly_figs.ipynb` produces the HTML outputs. Open it in VS Code or Jupyter, tweak parameters, re‑run, and export/save updated figures.

## Setup (Optional – only needed to regenerate)
Create a virtual environment and install dependencies listed in `requirements.txt`:

```fish
python3 -m venv .venv
source .venv/bin/activate.fish
pip install -r requirements.txt
```

Key libraries: Plotly (interactive graphs), NumPy (numerics), Jupyter (notebook runtime).


## Contributing
Add new figures under `interactive/mechanics/` or extend the notebook. Keep each figure self‑contained (no external CDN dependencies beyond what Plotly writes inline). Prefer clear filenames: `<concept>_<quantity>_vs_<quantity>.html`.

## Fast Reference
| Action | Command (fish) |
|--------|----------------|
| Open a figure | `open interactive/mechanics/net_force_vs_time_smooth.html` |
| Activate env | `source .venv/bin/activate.fish` |
| Install deps | `pip install -r requirements.txt` |
| Edit notebook | `open pcubed_plotly_figs.ipynb` (or launch via VS Code) |
