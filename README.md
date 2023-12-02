# Eagle Eye: Advanced Route Planning Solution for US Air Force

Eagle Eye is an innovative machine learning solution designed to streamline route planning for the US Air Force. This project leverages advanced predictive models and optimization techniques to enhance operational efficiency and decision-making.

## Key Features

- **Predictive Analysis**: Utilizes SARIMA, LSTMs, and Neuralprophet models to generate accurate airfield utilization predictions.
- **Optimization**: Implements linear programming optimization for effective route planning.
- **Scalable Architecture**: Designed to seamlessly integrate with existing systems and scale according to operational demands.

## Getting Started

Follow these steps to set up the Eagle Eye environment on your machine:

### Prerequisites

- Python 3.10.8
- Node.js and npm (for frontend setup)

### Installation

1. **Create a Conda Environment**:
   ```shell
   conda create --name eagle-eye python=3.10.8
   conda activate eagle-eye
2. **Install Python Dependencies:**
   ```shell
   pip install -r requirements.txt
3. **Run the Backend Server:**
   ```shell
   python api_fastapi.py
4. **Set Up the Frontend:**
    ```shell
    npm install
    npm start


## Version 0.4.0
### New Features
- Linked up 3 time-series utilization models to front end - now results are graphed through FastAPI
- Created a better map visualization using more modern tools
- Linked linear programming based route planning to a table at the bottom of the route planning page.
### Bug Fixes
- Fixed SARIMA bug where the resultant distribution would just be completely random
### Known Issues
- Models are not tuned and thus do not represent final performance (but better tuned than last time)
- neuralprophet model is trained on a different dataset and thus produces different results.

## Version 0.3.0
### New Features
- Created three models for airfield utilization time series prediction
- Created synthetic data generator to use in airfield utilization
- Created linear programming instance for fleet route planning
### Bug Fixes
- Fixed up bugs in the route planning visualization
### Known Issues
- Models are not tuned and thus do not represent final performance

## Version 0.2.0
### New Features
- Added business plot showing airfield ground clearance trends
- Added a file drop page for uploading new aifrield data
- Added flight route planning visualization in map component
### Bug Fixes
- Modularized airfield and business data from their respective components
### Known Issues
- Map view can be buggy rendering between frames

## Version 0.1.0
### New Features
- Added Dropdown menu for Airfields
- Added Map component for route planning
- Created centralized dashboard for flight stats
### Bug Fixes
- Refactored Artifact code to ensure variables were properly tracked across Dashboard tabs 
### Known Issues
- Hardcoded airfield data
