# Open Source Material for ISC2 Certified in Cybersecurity (CC)

This repository provides open-source study materials for the ISC2 Certified in Cybersecurity (CC) certification. The goal is to create a collaborative and accessible resource for anyone looking to learn about cybersecurity and prepare for the exam.

These materials are structured as slide decks using Markdown and are intended to be rendered with [Marp](https://marp.app/).

## Structure

The content is organized into folders corresponding to the official ISC2 CC domains:

-   **/Domain1:** Security Principles
-   **/Domain2:** Business Continuity (BC), Disaster Recovery (DR) & Incident Response Concepts
-   **/Domain3:** Access Controls Concepts
-   **/Domain4:** Network Security
-   **/Domain5:** Security Operations

Each domain folder contains the Markdown file (`.md`) for the presentation slides.

## Usage with Marp

To view, present, or convert these materials into formats like PDF or PowerPoint, you will need to use the Marp CLI tool.

### Installation

First, [install Marp CLI](https://github.com/marp-team/marp-cli).

### Rendering Slides

Once Marp is installed, you can convert the Markdown files into your desired format. A custom theme, `greenbar.css`, is included in the `res` directory to style the slides.

Use the following command from the root of the project to convert a domain's Markdown file into a PDF:

```bash
marp -o Domain3/Domain3.pdf --theme res/greenbar.css --allow-local-files ./Domain3
```

### Command Breakdown:

-   `marp`: Executes the Marp CLI.
-   `-o <output_file>`: Specifies the output file name and format (e.g., `Domain3.pdf`, `Domain3.pptx`).
-   `--theme <path_to_css>`: Applies the custom CSS theme for styling. We use `res/greenbar.css`.
-   `--allow-local-files`: This is crucial for allowing Marp to access local images stored in the `res` subdirectories within each domain folder.
-   `./Domain3`: Specifies the input directory containing the Markdown file (`Domain3.md`) and its associated resources. Marp will automatically find the `.md` file.

## How to Contribute

Contributions are welcome! If you would like to improve the materials, please fork the repository, make your changes, and submit a pull request.

## Disclaimer

These materials in the repository is for sharing the knowledge without any commercial purpose. No liability and responsibility from authors and contributors.
