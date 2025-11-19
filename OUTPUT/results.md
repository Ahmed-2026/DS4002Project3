## Summary of Findings:
- Baseline CNN (Cat vs. Dog):
    - Achieved an accuracy of 98%, with high precision and recall for both cats and dogs.
    - the pretrained ResNet50 model was able to separate the two species extremely well with minimal training
- Augmented CNN (Cat vs. Dog):
    - Achieved 98% accuracy, showing that while augmentation improved robustness, it did not significantly increase classification accuracy
- Breed Classification (37 Classes):
    - the fine-tuned multiclass CNN reached an accuracy of 83%, with a macro F1-score of 0.83
- Overall, the pretrained CNN performed well on species-level classification and strongly on breed-level classification despite the challenge posed by 37 visually similar classes. This confirmes that fine-tuning a pretrained CNN is highly effective for both binary and multiclass pet image classification.
