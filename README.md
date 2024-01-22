# polar-pipeline-lite

## Overview

This web application provides a user-friendly interface for searching and filtering VCF (Variant Call Format), TSV, or CSV files. It includes a file browser, a parameter configuration page, and a protein figure generator. The application is encapsulated within a Docker container, simplifying the deployment process.

## Features

### VCF File Search and Filtering

#### File Browser
- Browse and select VCF files with ease.

#### Parameter Configuration
- Utilize a block structure to specify search criteria.
- Add multiple blocks to create complex filtering conditions.
- Specify column, operator, and value for each block.
- Retrieve rows meeting all block requirements in the final output.

### Protein Figure Generator

- Generate protein figures with customizable options:
  - Zygosity selection.
  - Determine whether alleles have the same structure.
  - Mark features of interest on the protein figure.

## Getting Started

To deploy the web application, follow these steps:

### Prerequisites

- Install Docker on your system: [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

### Build and Run

1. Download the repository as a zip or clone this repository:
   ```bash
   git clone https://github.com/parkerpayne/polar-pipeline-lite
   cd polar-pipeline-lite
   ```
2. In a terminal (PowerShell in Windows) build the Docker container:
   ```bash
   docker compose build
   ```
3. Run the container:
   ```bash
   docker compose up -d
   ```
4. Access the web application in your browser: [http://localhost:5001](http://localhost:5001)

5. Stop the webapp using:
   ```bash
   docker compose down
   ```

### Usage

#### File Search

1. Copy files or directories of files to input folder in the polar-pipeline-lite directory.
2. Navigate to file you wish to search in using the file browser.
3. Configure search parameters on the parameter configuration page.
4. Click search.

#### Protein Figure Generator

Configurations can be saved using the "Save Preset" button at the bottom of the page. They can then be reloaded using the "Load Preset" button at the top of the page.

### License
This project is licensed under the MIT License.
