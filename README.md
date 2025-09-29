# ❤️ Heart Disease Prediction

This project uses Machine Learning to predict whether a person has heart disease (**1**) or not (**0**) based on medical attributes.  
The trained model achieves **94% accuracy on the test set**.

---
## 🎥 Video Demo
[![Watch the video](https://img.youtube.com/vi/5VNQNGwLEjg/maxresdefault.jpg)](https://youtu.be/5VNQNGwLEjg)

## 📂 Project Structure
- **`dataProcessing.ipynb`** → Prepares the dataset, trains the model, and generates:
  - `heart_disease_model.pkl` → Trained machine learning model (it will be genrated after running dataProcessing.ipynb)
  - `heart_model_test_set.csv` → Processed test set for validation (it will be genrated after running dataProcessing.ipynb)
- **`prediction.ipynb`** → Loads the saved model and makes predictions on:
  - Provided test set (`heart_model_test_set.csv`)  
  - Custom user input (optional)
- **`heart.csv`** → Main data set
---

## 🚀 How to Run

1. **Run data processing and model training**  
   Execute **`dataProcessing.ipynb`** once.  
   This will generate:
   - `heart_disease_model.pkl`  
   - `heart_model_test_set.csv`  

2. **Make predictions**  
   - Open **`prediction.ipynb`**  
   - By default, it predicts using the prepared test set
   - You can copy code from here and paste in normal .py file it will run fine just make sure you have installed all library needed

3. **Use your own data (optional)**  
   - In `prediction.ipynb`, find the section with `user_data`  
   - Uncomment the `user_data` DataFrame and enter your own values:  

   ```python
   user_data = pd.DataFrame([{
       'Age': 55,
       'Sex': 'M',
       'ChestPainType': 'ATA',
       'RestingBP': 140,
       'Cholesterol': 250,
       'FastingBS': 0,
       'RestingECG': 'Normal',
       'MaxHR': 150,
       'ExerciseAngina': 'N',
       'Oldpeak': 1.5,
       'ST_Slope': 'Up'
   }])
   ```
  - Change new_data_prepared to user_data in the prediction variable

4. **📊 Model Performance**
   
   -Algorithm: Random Forest Classifier
   
   -Accuracy: 94% on test set
   
## ✅ Example Prediction

**Input:** Patient data with medical features  

**Output:**  
- `0` → No Heart Disease  
- `1` → Heart Disease Present  

## 🧑‍💻 Author  
Developed by [Adarsh-OPP](https://github.com/Adarsh-OPP)  
For more information contact on discord(adarsh0910)

## 📜 License  
This project is licensed under the **MIT License** – feel free to use, modify, and distribute it as per your needs.  

## 📦 Libraries Used

- pandas  
- joblib  
- numpy  
- scikit-learn  

