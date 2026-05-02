# Clean-Repo
## Custom Mihon Extension Repository (Proxy-Based)

This repository hosts a custom extension index for the Mihon/Tachiyomi ecosystem. It was built by reverse-engineering the structure and behavior of existing extension repositories and implementing a compatible format for personal use and experimentation.

### Overview

The repository provides a curated list of manga extensions through a custom `index.min.json`, allowing Mihon to discover and install extensions directly from this source. It replicates the expected repository schema and integrates with Mihon’s extension manager.

### Key Features

* **Custom Extension Index**
  A fully functional `index.min.json` file containing extension metadata compatible with Mihon.

* **Repository Metadata Configuration**
  Includes a properly structured `repo.json` with a valid `signingKeyFingerprint`, enabling seamless installation of extensions within Mihon.

* **Working Repository Integration**
  The repository can be added directly to Mihon via:

  ```
  https://raw.githubusercontent.com/Zeko2005/Clean-Repo/main/
  ```

* **Extension Hosting Structure**
  Implements the required `/apk` and `/icon` directory structure to comply with Mihon’s internal fetching logic.

* **Reverse-Engineered Compatibility**
  The project was developed by analyzing existing repositories (e.g., Keiyoushi) to ensure compatibility with Mihon’s expectations for:

  * URL structure
  * JSON schema
  * file resolution behavior

### Current Capabilities

* Successfully loads in Mihon as a valid extension repository
* Displays extension entries correctly
* Supports installation of hosted extension APKs
* Properly resolves and displays extension icons

### Ongoing Work

* Automating synchronization with upstream extension sources
* Building custom extension APKs with modified behavior (e.g., content filtering)
* Improving repository scalability and maintenance workflow

### Notes

This project is intended for educational and personal use. It demonstrates how Mihon extension repositories are structured and how extensions are distributed and managed.

---

