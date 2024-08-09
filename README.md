# Neural Networks with BranchyNet Principles in PyTorch

This repository contains various neural network implementations following the BranchyNet principles, built using PyTorch. Each network is organized into its own directory (e.g., `AlexNet`), allowing for modular development and easy experimentation. The project also includes tools for training, validating, and logging model performance using TensorBoard.

## Tech Stack

### Core Libraries:
- **PyTorch**: Used for building and training neural networks.
- **TorchVision**: Provides datasets and transformations for image processing.
- **TensorBoard**: Logs and visualizes metrics during training.

### Utility Libraries:
- **os**: For managing file paths and directories.
- **torch.optim**: Optimizers for training (e.g., Adam).
- **torch.nn.functional**: Provides functions for neural network operations.
- **torch.utils.data**: Manages data loading and batching.

## Jupyter Notebook Usage

The entire development process, from model definition to training and evaluation, is performed within Jupyter Notebooks. This setup allows for iterative development and immediate feedback, making it easier to debug and visualize the learning process.

### Running the Project

To run the project, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/hrushikesh-sam/Branchynet-pytorch.git
    cd Branchynet-pytorch
    ```

2. **Set Up Virtual Environment**:
    Navigate to the directory of the specific network you want to run (e.g., `AlexNet`):
    ```bash
    cd AlexNet
    ```
    Create and activate a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install Dependencies**:
    Install the required packages from the `requirements.txt` file:
    ```bash
    python3 -m pip install -r requirements.txt
    ```

4. **Run the Jupyter Notebook**:
    Launch Jupyter Notebook and open the corresponding `.ipynb` file:
    ```bash
    jupyter notebook
    ```
    Select the notebook file (e.g., `AlexNet.ipynb`) and run the cells to execute the training process.

## Structure

Each directory represents a different neural network model and contains:
- **Notebook**: A Jupyter Notebook (`.ipynb`) with the model definition, training loop, and evaluation code.
- **Model Definition**: A Python file containing the network architecture.
- **Training Script**: A script to start the training process.
- **`requirements.txt`**: Dependencies required for the specific network.

## BranchyNet Principles

BranchyNet introduces early exits in neural networks, allowing the model to terminate computation early for easy-to-classify inputs, improving efficiency. This project implements this concept by defining multiple branches within the network that can produce outputs at different depths.

## Contributions

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the GNU General Public License v3.0. See the `LICENSE` file for more details.
