# Princeton ORF522 Linear and Nonlinear Optimization Companion

Supporting material for [Princeton ORF522 course: Linear and Nonlinear Optimization](https://stellato.io/teaching/orf522)

## 🚀 Run in GitHub Codespaces

You can launch this environment directly in your browser with GitHub Codespaces:

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/orf522/companion)

### How to use

1. Click the badge above (requires a GitHub account).
2. Wait a couple of minutes while the Codespace starts.
3. In the Codespaces menu, go to **… → Open in → JupyterLab**.
4. You’ll be in a full JupyterLab environment with all the optimization and LaTeX packages preinstalled.
5. Work in the browser; your files persist in the Codespace.  
   Save to GitHub if you want permanent storage.

## 💾 Save your work locally (important!)

GitHub Codespaces are **temporary** workspaces:

- A codespace **stops** after ~30 minutes of inactivity (you can change this in your own GitHub settings). [GitHub Docs](https://docs.github.com/en/codespaces/setting-your-user-preferences/setting-your-timeout-period-for-github-codespaces)
- **Stopped** codespaces are **automatically deleted after up to 30 days** of inactivity (that retention can be shorter if you’ve set it in your GitHub account). [GitHub Docs](https://docs.github.com/en/codespaces/about-codespaces/understanding-the-codespace-lifecycle)

➡️ **Before you close the browser or step away**, download your files to your computer:

**From JupyterLab**

1. Right-click a file/folder in the left sidebar → **Download**.
2. For many files at once, you can zip a folder in the terminal and download the zip:
   ```bash
   zip -r work.zip .
   ```

Then right-click work.zip → Download.

Tip: Codespaces persist between sessions until they’re deleted by the retention policy, but do not rely on them for long-term storage. Always keep a local copy or push to a repo you own.

## Troubleshooting

- `Failed to process string with tex because latex could not be found` when generating plots.
  You most likely do not have latex installed (not present by default in colab). You can simply fix this by commenting the line:

  ```python
  # "text.usetex": True,
  ```

- `AttributeError: 'Axes3D' object has no property 'auto_add_to_figure'` when generating the simplex 3D plots.
  You most-likely have an older version of `matplotlib` installed. You can just create a new cell and run `!pip install -U matplotlib` (remember to restart your runtime/kernel to activate the changes).
