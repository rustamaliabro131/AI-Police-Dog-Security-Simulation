# AI-Police-Dog-Security-Simulation
A Python-based autonomous security simulation designed for high-risk industrial zones. This project demonstrates complex AI behaviors, including real-time pathfinding, intruder detection, and intelligent power management.
Key Features:
* FSM-Driven AI: Seamless transitions between patrolling, chasing, and self-docking.
* Tactical Telemetry: Real-time monitoring of battery life, speed, and unit status.
* Fail-Safe Protocols: Auto-return-to-base logic to prevent unit shutdown in the field.
* Simulated Locomotion: Mathematical sway simulation for realistic legged movement.
* Project Roadmap
1. Obstacle Avoidance (Ray-Casting)Currently, the dog can "walk through" static objects. To fix this, you should implement basic ray casting or A* pathfinding. The Goal: Add "Industrial Shelving" or "Static Blocks" to the simulation.The Logic: Before moving, the dog should "look" ahead; if an obstacle is detected, it should recalculate its path to go around it rather than through it.🏃
2. Variable Thief AI (Smart Intruder)Your roadmap suggests upgrading the intruder logic from random movement to goal-oriented movement. The Logic: When the dog's DETECTION_RADIUS is triggered, the Thief entity should identify the nearest "Exit" coordinate and prioritize moving toward it to escape.The Challenge: This creates a "Cat and Mouse" dynamic where the dog must catch the thief before they reach the exit.🔋
3. Energy Fail-Safe Validation: Your milestone tracker shows that while Pursuit and Patrol are "Stable," the Energy Fail-Safe is still "In-Dev".Stress Test: Run simulation loops to ensure the dog successfully abandons a chase when the battery hits $20\%$ and consistently reaches the dock at $(50, 50)$ without dying.Visual Feedback: Ensure the unit turns orange during the CHARGING state as planned.
