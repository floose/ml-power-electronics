# Continue in VS Code

The cloud virtual environment and `/workspace/.cloud-setup` helpers are outside
the repository and do not travel with a Git clone. Recreate the environment
locally; the commands below use the top-level versions validated in the cloud,
but do not lock transitive dependencies across operating systems.

1. Install Python 3.12 and the VS Code Python and Jupyter extensions.
2. Open this repository in VS Code and create an environment:

   ```sh
   python -m venv .venv
   ```

3. Activate it on Linux/macOS with `source .venv/bin/activate`, or on Windows
   PowerShell with `.venv\Scripts\Activate.ps1`.
4. Install the research tools:

   ```sh
   python -m pip install numpy==2.5.4 scipy==1.18.1 matplotlib==3.11.2 scikit-learn==1.9.1 jupyterlab==4.6.4 pytest==9.1.1
   python -m pip install torch==2.14.1 --index-url https://download.pytorch.org/whl/cpu
   python -m pip check
   ```

   The PyTorch command targets supported Linux/Windows CPU wheels. On macOS,
   install `torch==2.14.1` from PyPI instead. Local installation and Apple MPS
   have not been validated; use the official PyTorch installation guidance if
   a wheel is unavailable for your platform. Cloud checks used CPU only.

5. Run **Python: Select Interpreter** and select `.venv`. For notebooks, select
   the same environment as the kernel.
6. Keep `.venv` out of commits. Read `Agents.md` and `docs/progress.md` before
   beginning experiments. There is no project test suite or study plan yet.

The cloud validated dependency consistency, numerical integration, regression,
plotting, PyTorch training, notebook execution and JupyterLab startup. Repeat
relevant functional checks locally before claiming local readiness.
