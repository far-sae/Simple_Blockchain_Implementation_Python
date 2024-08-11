
# Simple Blockchain Implementation in Python

## Overview

This project provides a basic implementation of a blockchain in Python. The blockchain is a decentralized digital ledger used to record transactions across many computers so that the record cannot be altered retroactively. This implementation includes fundamental features such as block creation, proof of work, and basic API endpoints to interact with the blockchain.

## Features

- **Block Creation**: Each block in the blockchain contains an index, timestamp, proof, and the hash of the previous block.
- **Proof of Work**: The implementation includes a simple proof of work algorithm to secure the network.
- **Blockchain Management**: Functions to retrieve the previous block and to add new blocks to the chain.
- **API Interface**: A basic Flask server is provided to interact with the blockchain via HTTP requests.

## Project Structure

- `blockchain.py`: The main script that contains the `Blockchain` class and its associated methods.
- **Flask API**: The script uses Flask to create a simple API for interacting with the blockchain.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/far-sae/Simple-Blockchain_Implementation_Python.git
    ```
2. **Navigate to the project directory**:
    ```bash
    cd Simple-Blockchain_Implementation_Python
    ```
3. **Install the required dependencies**:
    ```bash
    pip install flask
    ```

## Usage

1. **Run the Flask server**:
    ```bash
    python blockchain.py
    ```
2. **Interact with the blockchain**:
    - **Mine a new block**:
      ```bash
      GET /mine_block
      ```
    - **Get the full blockchain**:
      ```bash
      GET /get_chain
      ```
    - **Check if the blockchain is valid**:
      ```bash
      GET /is_valid
      ```

## Example Requests

- **Mine a block**:
    ```bash
    curl http://127.0.0.1:5000/mine_block
    ```
- **Get the blockchain**:
    ```bash
    curl http://127.0.0.1:5000/get_chain
    ```
- **Check if the blockchain is valid**:
    ```bash
    curl http://127.0.0.1:5000/is_valid
    ```

