# RADGN
# Paper Title:
Interpretable Reaction-Aware Graph Learning for Rapid Screening of Liquid Organic Hydrogen Carriers
# Highlights
	1.Reaction-aware dual-graph GNNs predict LOHC dehydrogenation enthalpy from QM9-G4MP2. 
	2.D-MPNN+XGB attains test MAE of 3.70 kJ/mol and R² = 0.94 across 10,345 reaction pairs. 
	3.Hybrid-RADGN gives lowest error (4.20 kJ/mol) inside the 40–70 kJ/mol design window. 
	4.LOHC-aware weighted Huber loss targets the practical hydrogen-release operating range. 
	5.SHAP shows ΔLogP and learned embeddings dominate enthalpy prediction.

# Abstract
The development of efficient Liquid Organic Hydrogen Carriers (LOHCs) is critical for enabling safe and practical hydrogen storage and transportation. A key factor in LOHC selection is the accurate prediction of dehydrogenation enthalpy (ΔH), which determines the energy required for hydrogen release. Computationally expensive high level quantum chemical methods offer reliable predictions, but are restricted to large scale screening of molecules. This study proposes two reaction-aware machine learning (ML) frameworks, Hybrid-RADGN and D-MPNN+XGB, for predicting LOHC dehydrogenation enthalpies using the QM9-G4MP2 dataset containing 10,345 reaction pairs. Both models were individually trained to encode hydrogen-rich and hydrogen-poor molecular structures, and combined graph-based molecular representations with physicochemical reaction-difference descriptors. Hybrid-RADGN used a dual-graph attention network and shared the weights with a reaction-level embedding, while D-MPNN+XGB used directed message-passing neural network embeddings and XGBoost regression. The models were evaluated using 5-fold cross-validation and benchmarked against twelve baseline machine learning and graph neural network methods. The results show that D-MPNN+XGB achieved the highest overall predictive performance, with a test MAE of 3.700 kJ mol⁻¹ and R² of 0.9408, whereas Hybrid-RADGN provided the best accuracy within the practical LOHC operating window of 40-70 kJ mol⁻¹, with an MAE of 4.203 kJ mol⁻¹. SHAP based interpretation revealed that the change in molecular lipophilicity (ΔLogP) and learned graph embeddings are the most influential predictors. The proposed frameworks offer accurate, interpretable, and computationally efficient tools for accelerating the discovery and screening of next-generation LOHC materials.
