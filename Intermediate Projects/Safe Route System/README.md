SafeRoute — AI-Powered Smart Route Safety Analyzer

A desktop application that analyzes route safety using:
✔ CSV-based safety dataset
✔ AI-trained linear model
✔ Baseline heuristic scoring
✔ Real-time GPS route simulation
✔ Safety heatmap visualization
✔ Tkinter-based interactive GUI

This project blends Machine Learning, Data Processing, Visualization, and GUI development into a complete intermediate–advanced level Python project.

📌 Features
1. CSV Route Safety Loader
Loads route data from CSV (supports flexible column names).
Reads fields like:
Crime Rate
Lighting
CCTV Count
Crowd Density
Safety Score (optional)
Automatically handles missing or malformed values.

3. Baseline Scoring System
Every route gets a handcrafted safety score based on:
Low crime
Good lighting
More CCTV
High crowd presence
Used when CSV does not contain a safety score.

3. AI Scorer — Tiny Linear Regression Model
A fully from-scratch machine learning model.
Normalizes input features
Gradient descent training
Predicts a smarter AI-based safety score
Lets users compare routes using ML predictions.

4. GPS Route Simulation

Enter coordinates like:
Start: 12.95,77.59  
End:   12.97,77.60

The app then:
Generates interpolation points
Simulates safety values using noise + sinusoidal patterns
Renders a heatmap path on canvas
Color codes each point:

🔴 Red → dangerous
🟢 Green → safe

5. Full Tkinter GUI Application

Includes:

CSV loader
Route selectors
Baseline comparison
AI comparison
Simulation controls
Heatmap canvas
Status bar

Everything is interactive and polished.

🗂️ Project Structure
│── Safe Route System.py         
│── sample.csv                     
│── README.md                     

📥 CSV Format

Your CSV can contain ANY of these names; the loader will detect them:

Route columns (any one):
route, route_name, name, route id

Safety feature columns:
crime_rate, crime
lighting, light
cctv, cameras
crowd, density

Optional safety score column:
safety, safety_score, score


If safety score is missing → model will use baseline score as label.

🚀 How to Run
1. Install Python 3.7+
Check your version:
python --version

2. Run the application
python safe_route.py

The GUI will launch immediately.

🎛️ Using the Application
1. Load CSV
Click Open CSV → Select file
Routes populate automatically.

2. Compare Routes (Baseline Method)
Select two routes
Click Compare (baseline)

3. Train AI Model

Click Train AI scorer
Uses CSV data to build prediction model.

4. Compare with AI
Click Compare (AI model)
Shows ML-generated safety scores.

5. GPS Simulation

Enter:
lat1,lon1
lat2,lon2

Click Simulate Route & Heatmap
Heatmap draws automatically.

🧠 Machine Learning Model Details
Model: Custom Linear Regression
Optimization: Gradient Descent
Input features:
Bias
(10 - Crime Rate)
Lighting
CCTV
Crowd
Normalization: mean–std scaling
Loss: Mean Squared Error
Implementation: Fully manual (no sklearn used)
This makes it an excellent educational ML project.

📸 Heatmap Output
Green → High Safety
Red → Low Safety
Path plotted using interpolated GPS points
Canvas auto-scaled based on coordinates

🔧 Advanced Features
Robust CSV parsing
Error handling for all user inputs
Flexible header detection
Automatic default values for missing fields
Clean UI layout with ttk widgets
Full separation of Model, Analyzer, and GUI
