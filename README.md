# Train RL agents to play Pokemon Red
Code to train reinforced learning agents to play the GameBoy game Pokemon Red

Requirements
- Pokemon Red ROM in base directory, name it "PokemonRed.gb"
- sha1 sum is "ea9bcae617fdf159b045185467ae58b2e4a48b9a", run "shasum PokemonRed.gb" to check
- install dependencies with "pip install -r requirements.txt" in baselines subfolder
- run "python run_pretrained_interactive.py"
  
Notes
Use arrow keys and A and S keys for the A and B buttons
You can pause the AI inputs by editing the "agent_enabled.txt"
pokemon.gb file must be in main directory, remember to be in the baselines directory

# Train the Model  

This version still needs some tuning, but it can clear the first gym in a small fraction of the time and compute resources. It can work with as few as 16 cores and ~20G of RAM. This is the place for active development and updates! 

1. Previous steps 1-3
2. Run:  
```python run_baseline_parallel_fast.py```

Current state of each game rendered in images in session directory
Run "tensorboard --logdir" to track the progress in tensorboard, go to "localhost:6006" to view metrics

Map visualization code can be found in "visualization" directory.

Libraries Used
PyBoy
StableBaselines 3