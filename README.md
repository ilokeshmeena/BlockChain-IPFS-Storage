# BlockChain-IPFS-Storage

This repository contains a blockchain-based storage solution built with **IPFS (InterPlanetary File System)** and **Node.js**. It leverages the decentralized nature of blockchain for secure and efficient file storage. Docker is used for containerizing the application for easy deployment and scalability.

## Features

- **Decentralized Storage**: Utilizes IPFS to store files in a decentralized manner.
- **Blockchain Integration**: Ensures security and immutability of file metadata using blockchain.
- **Docker Support**: Containerized using Docker to enable fast setup and consistent environments.
- **Node.js Backend**: Powered by Node.js for handling IPFS file operations and blockchain transactions.

## Prerequisites

Before you start, make sure you have the following installed:

- [Node.js](https://nodejs.org/en/) (version 14 or higher)
- [Docker](https://www.docker.com/get-started)
- [IPFS CLI](https://docs.ipfs.tech/install/) (optional, for managing IPFS nodes directly)

## Getting Started

1. **Clone the repository:**

    ```bash
    git clone https://github.com/ilokeshmeena/BlockChain-IPFS-Storage.git
    cd BlockChain-IPFS-Storage
    ```

2. **Install Node.js dependencies:**

    ```bash
    npm install
    ```

3. **Build and run the Docker container:**

    Ensure Docker is running on your machine, then:

    ```bash
    docker build -t blockchain-ipfs-storage .
    docker run -p 3000:3000 blockchain-ipfs-storage
    ```

4. **Start the IPFS daemon (if not running already):**

    You can run the IPFS daemon locally:

    ```bash
    ipfs daemon
    ```

5. **Access the Application:**

    Once the container is up and running, you can access the app at [http://localhost:3000](http://localhost:3000).

## Project Structure

- **/src**: Contains the Node.js source code for handling IPFS operations and blockchain logic.
- **/Dockerfile**: Docker configuration file for containerizing the application.
- **/package.json**: Node.js project configuration file containing dependencies and scripts.

## Usage

- Upload files to the IPFS network via the web interface or API.
- The file's metadata is stored on the blockchain for security and auditability.

## Running Tests

To run tests, use the following command:

```bash
npm test
```

## Docker Details

- The application runs in a Node.js Docker container.
- Docker ensures consistency between environments and simplifies deployment.

To stop and remove the container:

```bash
docker stop <container_id>
docker rm <container_id>
```

## Contributing

Feel free to submit issues or pull requests. Contributions are welcome!

---

Let me know if you want any additional sections or modifications!
