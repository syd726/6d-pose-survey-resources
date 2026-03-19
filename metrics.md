# Evaluation Metrics

## ADD
- Full name: Average Distance of Model Points
- Description: ADD measures the average distance between model points transformed by the estimated pose and those transformed by the ground-truth pose. It is one of the most widely used metrics for evaluating 6D object pose estimation accuracy.
- Typical Usage: Commonly used for asymmetric rigid objects.
- Note: In practical evaluation, the estimated pose is often considered correct when the ADD value is smaller than a predefined fraction of the object diameter, such as 10%, 5%, or 1%.

## ADD-S
- Full name: Average Distance for Symmetric Objects
- Description: ADD-S is a variant of ADD designed for symmetric objects. Instead of enforcing one-to-one point correspondence, it computes the average distance from each transformed model point to its closest point in the other pose-transformed model set.
- Typical Usage: Suitable for symmetric or partially symmetric objects, where standard ADD may be overly strict.
- Note: Similar to ADD, threshold-based evaluation is commonly adopted using a fraction of the object diameter.

## VSD
- Full name: Visible Surface Discrepancy
- Description: VSD evaluates the discrepancy between the visible object surfaces rendered under the estimated pose and the ground-truth pose. It is designed to reduce ambiguity caused by object symmetry and occlusion.
- Typical Usage: Particularly suitable for occluded scenes and benchmark evaluations such as BOP.
- Note: VSD focuses on visible regions rather than the full object surface, making it more robust in heavily occluded scenarios.

## AR
- Full name: Average Recall
- Description: AR is a comprehensive evaluation metric widely used in BOP-style benchmarks. It summarizes recall values under multiple error thresholds and may integrate different pose-error criteria such as VSD, MSSD, and MSPD.
- Typical Usage: Used for benchmark-style overall performance evaluation across multiple thresholds and error definitions.
- Note: A higher AR value indicates better overall pose estimation performance.

## 2D Projection Metric
- Description: This metric measures the average distance between the 2D projections of model points under the estimated pose and those under the ground-truth pose in the image plane.
- Typical Usage: Commonly used in image-based 6D pose estimation tasks.
- Note: In many studies, a pose is considered correct when the average projection error is below a fixed pixel threshold, such as 5 pixels.

## n°mcm Metric
- Description: The n°mcm metric evaluates pose estimation using dual constraints on rotation error and translation error. A pose is regarded as correct only when both the rotation error and the translation error are below preset thresholds.
- Typical Usage: Common configurations include 5°5cm and 5°10cm, depending on the required precision of the application.
- Note: This metric is intuitive and practical, and is often used to evaluate the effectiveness of pose estimation methods in real-world scenarios.
