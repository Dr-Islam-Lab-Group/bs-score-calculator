# bs-score-calculator

Features

- Interactive **Binding Score (BS)** calculation
- Real-time updates as parameters change
- Clear breakdown of formula components
- **2D Tanimoto similarity** calculation from SMILES
- Automatic addition of similarity-derived values into **Sᵢ**
- Clean, responsive UI (no frameworks required)

---

## 🧮 Binding Score Formula

The calculator uses the following formula:


### Parameters

| Symbol | Description |
|------|-------------|
| **Rᵢ** | Ratio of molecules |
| **Smax** | Maximum similarity |
| **Sᵢ** | Indivual Similarity  |
| **w** | Weight (0–1) balancing similarity vs exponential term |
| **A** | Binding Affinity |
| **β** | Decay constant (must be > 0) |



## 2D Tanimoto Similarity

- Enter a **SMILES string**
- The app calls a local API to compute **Tanimoto similarity**
- The similarity value is scaled to `0–100`
- The result is **automatically added to Sᵢ**
