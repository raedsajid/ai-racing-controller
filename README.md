# ai-racing-controller
Autonomous AI racing controller for TORCS simulator using Python and telemetry-based logic.

## Structure
```
src/
├── ai_controller.py      # Entry point
├── driver.py             # Main logic for decision-making
├── carState.py           # Sensor data interpreter
├── carControl.py         # Generates control commands
├── msgParser.py          # Handles simulator messages
├── clean_csv.py          # Optional data utility
```

## Setup

1. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Client

Make sure the simulator is running and listening for input.

Then run the controller:
```bash
python src/ai_controller.py
```

## Notes

- Ensure the simulator (e.g., TORCS) is properly configured.
- Edit parameters in `driver.py` to fine-tune behavior.
