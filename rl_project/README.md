# DQN Space Invaders Project

This project implements a Deep Q-Network (DQN) agent to play the Atari game Space Invaders.

## 1. Environment Setup

### 1.1. Local Environment Setup (Placeholder)

(Details for local setup need to be provided by the user. This section is a placeholder.)

*   Python version: (e.g., 3.8+)
*   Virtual environment tool: (e.g., venv, conda)
*   Steps:
    1.  Clone the repository.
    2.  Navigate to the project directory.
    3.  Create and activate a virtual environment.
    4.  Install dependencies (see section 1.4).

### 1.3. Google Colab Setup

1.  **Upload to Google Drive:**
    *   Upload the `rl_project` folder (containing the `dqn_spaceinvaders.ipynb` notebook and this README) to your Google Drive.
2.  **Open in Colab:**
    *   Navigate to Google Colab.
    *   Open the `dqn_spaceinvaders.ipynb` notebook from your Google Drive.
3.  **Mount Drive:**
    *   The notebook contains a cell to mount your Google Drive. Run this cell and authorize access. This will allow the notebook to access files in your Drive.
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
    *   Make sure to update any file paths in the notebook to point to the correct location in your mounted Drive (e.g., `/content/drive/My Drive/rl_project/`).

### 1.4. Install Librerías Necesarias (Required Libraries)

The following libraries are required. You can install them using pip:

```bash
pip install tensorflow  # Or your preferred deep learning library like pytorch
pip install gymnasium[atari,accept-rom-license]
pip install numpy
pip install matplotlib
```

In Google Colab, you can run these commands in a code cell by prefixing them with `!`:

```python
!pip install tensorflow
!pip install gymnasium[atari,accept-rom-license]
!pip install numpy
!pip install matplotlib
```

## 2. Project Goal

The primary goal is to train a DQN agent that achieves an average reward of **over 20 points** in test mode when playing SpaceInvaders-v0.

## 3. Running the Notebook

1.  Ensure your environment is set up and libraries are installed (Section 1).
2.  If using Colab, mount your Google Drive (Section 1.3).
3.  Open and run the cells in `dqn_spaceinvaders.ipynb` sequentially.
    *   **Environment Setup Cells:** Install libraries and mount Drive (if in Colab).
    *   **DQN Implementation Cells:** Define the agent, neural network, and replay buffer.
    *   **Training Cell:** Run the training loop. This may take a significant amount of time.
    *   **Testing Cell:** Evaluate the trained agent's performance. The average reward will be printed.
