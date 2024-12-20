# Computing-in-Healthcare

## Project Title: Genomic Data Classification with Deep Learning

### Description
This project is divided into two phases, each focusing on genomic data preprocessing and classification using deep learning techniques. The ultimate goal is to classify genomic sequences as DNA-accessible (label 1) or DNA-inaccessible (label 0) using models such as AlexNet and NiN.

---

### Phase 1: Data Preparation

#### Objectives
- Extract and preprocess genomic data for classification tasks.
- Generate output files containing DNA-accessible and DNA-inaccessible sequences.

#### Tasks
1. Generate 20 output files (10 DNA-accessible and 10 DNA-inaccessible sequences) or two consolidated files.
2. Preprocess data into a suitable format for machine learning workflows.

---

### Phase 2: Model Training and Evaluation

#### Objectives
- Implement custom data loaders to process genomic data.
- Train and evaluate deep learning models for classification.

#### Steps
1. **Data Labeling:**
   - Assign labels to sequences: 1 for DNA-accessible and 0 for DNA-inaccessible.
2. **Data Consolidation:**
   - Combine the generated files into one consolidated dataset with labels.
   - Optionally create a smaller subset for practice (e.g., 1,000 data points).
3. **One-Hot Encoding:**
   - Convert sequences into one-hot-encoded arrays, preferably as NumPy arrays.
   - Separate data and labels (e.g., `data[0]` for sequence and `data[1]` for label).
4. **Tensor Conversion:**
   - Transform one-hot-encoded data into tensor format for PyTorch.
5. **Custom Data Loader:**
   - Implement a data class and create a custom data loader with shuffling enabled for training.
6. **Data Splitting:**
   - Split data into 80% training and 20% testing datasets.
7. **Model Training:**
   - Train models using 1D CNN architecture (AlexNet and NiN) for 5 epochs.
   - Experiment with two sets of hyperparameters for each model, with a focus on optimizing hidden layers and execution speed.
8. **Experiment Runs:**
   - Conduct four experiment runs:
     - AlexNet with two different hyperparameter sets.
     - NiN with two different hyperparameter sets.
   - Use a minimum of 10,000 data points for each experiment.
9. **Evaluation Metrics:**
   - Plot accuracy vs. epoch graphs (four curves in a single plot).
   - Create confusion matrices for each experiment.

---

### Requirements
- **Python Libraries:**
  - PyTorch
  - NumPy
  - Matplotlib
  - Additional libraries for data processing and visualization

- **Input Data:**
  - Output files from Phase 1 (DNA-accessible and DNA-inaccessible sequences).

---

### Rubric
1. **Custom Data Loader:**
   - Successfully implemented with one-hot-encoded data (150 points).
2. **Model Training:**
   - Models (AlexNet and NiN) trained and evaluated.
3. **Visualization:**
   - Accuracy vs. epoch graph (25 points).
   - Confusion matrix (25 points).
4. **Submission:**
   - Upload all relevant files to Moodle.
   - Attend one-on-one interview to discuss implementation.

---

### Important Notes
- Ensure your implementation is unique and adheres to the guidelines.
- Use a minimum of 10,000 data points for robust experiments.
- Enable `shuffle=True` for training datasets in PyTorch.
- Failure to upload code and subsets of data will result in significant penalties.

---

### License
This project is licensed for educational purposes only.

