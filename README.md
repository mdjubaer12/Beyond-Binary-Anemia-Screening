# Beyond-Binary-Anemia-Screening
# ABSTRACT
Most automated anemia screening systems classify patients as Anemic or Non-Anemic, a binary
design that structurally ignores compensated microcytic phenotypes characteristic of thalassemia
trait. This study presents an explainable tri-class complete blood count (CBC)-based machine
learning framework distinguishing Anemic, Compensated Microcytosis (CM), and Non-Anemic
patients, evaluated on the multicenter TriHemo-MCV dataset (n = 5,037; four tertiary hospitals,
Bangladesh). Four classifiers (Logistic Regression, Random Forest, XGBoost, and LightGBM) were
benchmarkedagainstthree classical hematological discrimination indices under 5-fold stratified cross
validation and held-out test evaluation; a dedicated leakage-free experiment excluded hemoglobin
derived variables, and SHAP analysis was applied to both feature sets for interpretability. Binary
classification incorrectly labeled 71.9% of CM patients as Non-Anemic. In the full-feature setting,
gradient boosting models achieved near-perfect cross-validation performance and complete held
out classification (𝜅 = 1.000); the leakage-free reduced model retained 79.5% accuracy without
hemoglobin-derived inputs, and LightGBM achieved a 2.24-fold improvement in CM sensitivity over
the best-performing classical index. SHAP analysis identified red blood cell (RBC) count and red cell
distribution width-coefficient of variation (RDW-CV) as the dominant independent CM predictors,
consistent with the pathophysiology of compensated thalassemia trait. Because CM labels are defined
by CBC hematological thresholds rather than HbA2 confirmation, the framework is intended as a pre
screening triage tool to identify individuals warranting confirmatory HbA2 testing, not as a standalone
diagnostic. The proposed approach is interpretable, computationally lightweight, and particularly
suitable for resource-limited settings.
