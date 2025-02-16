# AIAGENT
# HealthBot - A Healthcare Assistant

## Overview
HealthBot is an AI-powered healthcare assistant that can:
- Calculate Body Mass Index (BMI) based on weight and height.
- Analyze symptoms and suggest possible health conditions.
- Provide a friendly and interactive chatbot experience.

Access bot using below link:
https://huggingface.co/spaces/hemantgaikwad/First_agent_template

## Features
1. **BMI Calculation:**
   - Accepts weight (kg) and height (m) as inputs.
   - Calculates BMI and provides health status (underweight, normal, overweight, or obese).

2. **Symptom Analysis:**
   - Accepts a comma-separated list of symptoms.
   - Matches symptoms to possible conditions and provides recommendations.

3. **Interactive Chatbot:**
   - Greets users with "Welcome to HealthBot! How can I assist you today?"
   - Handles unknown symptoms gracefully.

## Installation
To run HealthBot, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd healthbot
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application:**
   ```bash
   python app.py
   ```

## Usage
### **1. BMI Calculation**
#### Example Input:
```
calculate_bmi 70 1.75
```
#### Expected Output:
```
Your BMI is 22.86, which is considered normal weight.
```

### **2. Symptom Analysis**
#### Example Input:
```
analyze_symptoms fever, cough
```
#### Expected Output:
```
Based on your symptoms (fever, cough), you may have: Possible Flu or COVID-19. Consult a doctor for a proper diagnosis.
```

### **3. General Interaction**
#### Example Input:
```
Hello
```
#### Expected Output:
```
Welcome to HealthBot! How can I assist you today?
```

## Configuration
- The agent is powered by `Qwen/Qwen2.5-Coder-32B-Instruct`.
- The chatbot uses a predefined YAML file (`prompts.yaml`) for structured responses.
- The chatbot is deployed via `GradioUI`.

## Troubleshooting
- If `GradioUI` does not accept `initial_message`, remove the argument when launching the chatbot.
- Ensure all dependencies are installed using the `requirements.txt` file.

## Future Enhancements
- Integrate a more advanced symptom diagnosis system.
- Add support for real-time medical advice via APIs.
- Implement voice-based interactions.

## Disclaimer
**HealthBot is not a substitute for professional medical advice. Always consult a healthcare provider for accurate diagnosis and treatment.**

---

Developed by: [Your Name]  
Contact: [Your Email]

