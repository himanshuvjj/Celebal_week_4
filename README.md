
###  EDA Conclusion and Analysis – *Smartphones Dataset*

Based on your Jupyter notebook, here is a structured summary of the **EDA insights and final analysis**:

---

###  **1. Data Overview**

* The dataset was loaded successfully, with a variety of features like:

  * `has_5g`, `nfc`, `num_rear_cameras`, `extended_memory_available`, `processor_speed`, etc.
* Missing values were present and handled using **machine learning-based imputation (IterativeImputer + RandomForestRegressor)** for numerical features and **mode imputation** for categorical features.

---

###  **2. Univariate Analysis**

* Variables like `processor_speed`, `num_rear_cameras`, and `extended_memory_available` were explored individually.
* These showed diversity in smartphone hardware and software configurations.

---

###  **3. Bivariate Analysis**

* Focused on `has_5g` vs:

  * `nfc`
  * `num_rear_cameras`
  * `extended_memory_available`

####  **Key Observations**:

* **NFC vs 5G**:

  * Many phones **have 5G but no NFC** (214 devices).
  * Few phones **have NFC but no 5G** (58 devices).
  *  **Insight**: 5G is becoming more common across budget to premium phones, while NFC remains a premium or niche feature.

* **Rear Cameras vs 5G**:

  * 5G phones tend to have **more rear cameras**, especially peaking at **3 cameras**.
  *  **Insight**: Brands are combining 5G with richer camera setups in mid and high-end segments.

* **Expandable Memory vs 5G**:

  * Newer 5G phones often **do not offer expandable storage**.
  * **Insight**: Reflects industry trends toward larger internal storage and sleeker designs without SD card slots.

---

 **Overall Conclusion**

* **5G availability correlates strongly with modern features** like multiple cameras and no expandable storage.
* **NFC** is not yet widespread among 5G phones, indicating it's not a priority for all manufacturers.
* Brands are aligning **hardware complexity (e.g., multi-camera, fast processors)** with **5G support** to define flagship and upper mid-range models.
* Feature trends reflect broader **industry shifts**—e.g., phasing out expandable memory and prioritizing internal capacity.
