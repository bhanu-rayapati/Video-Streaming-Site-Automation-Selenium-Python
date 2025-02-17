# Video-Streaming-Site-Automation-Selenium-Python-BDD-Framework

Welcome to the **Video Streaming Site Automation Framework**, a robust test automation solution designed for video streaming platforms. This framework leverages **Selenium**, **Python**, and **Pytest-BDD** to automate end-to-end user journeys, including login, video playback, volume control, resolution changes, and logout.


## 🚀 Key Features

- **Behavior-Driven Development (BDD)**:  
  - Test scenarios written in **Gherkin syntax** for clear, business-readable specifications.
- **Page Object Model (POM)**:  
  - Clean separation of UI locators and test logic for maintainability.
- **Cross-Browser Testing**:  
  - Supports **Chrome**, **Firefox**, and **Edge** for multi-browser compatibility.
- **Dynamic Test Data Management**:  
  - Configurable test data through `config.ini` and external data sources.
- **Video Playback Testing**:  
  - Specialized handlers for play, pause, replay, volume and resolution changes.
- **Smart Waits**:  
  - Automatic synchronization with dynamic web elements.

## 🗂️ Framework Structure
Here's the framework structure:
```
📁 Video-Streaming-Automation/
│
├── 📁 features/
│   └── video_playback.feature      # Gherkin test scenarios
├── 📁 step_definitions/
│   └── test_video_steps.py         # BDD step implementations
├── 📁 page_objects/
│   ├── base_page.py                # Core Selenium operations
│   ├── login_page.py               # Password authentication handling
│   └── video_page.py               # Video controls implementation
├── 📁 tests/
│   ├── test_video_playback.py      # This test file integrates with Pytest-BDD to load the Gherkin feature scenarios defined in the 'video_playback.feature' file located in the features directory.
├── 📁 config/
│   └── config.ini                  # Environment configurations
├── 📁 utilities/
│   ├── driver_manager.py           # Browser factory
│   └── config_reader.py            # INI file parser
├── 📁 test-output/
│   ├── screenshots/                # Failure captures
│   └── report/                     # Raw report data
```

## 📜 Prerequisites

- **Python 3.x** 
- **Selenium**
- **Pytest-BDD** 


## 🛠️ Installation

1. Clone this repository:
    ```bash
     git clone https://github.com/bhanu-rayapati/video-streaming-automation.git]
    ```

2.  Install dependencies:

    ```
    pip install selenium
    pip install configparser  # If using config.ini
    ```

3.  Configure `config.ini`:

    *   Update the `config.ini` file with the appropriate values for your environment (URLs, credentials, etc.).
  
## 🧪 Running the Tests

Example using pytest (you'd need to install pytest and create test files in a `tests` directory):

1.  **Install pytest:**

    ```
    pip install pytest
    ```

2.  **Create test files:**

    *   (e.g., `tests/test_login.py`, `tests/test_video_playback.py`)

3.  **Run the tests:**

    ```
    pytest
    ```

