# Amazon-Fashion-Recommendation
Used Amazon Product Advertising API to gather data locally and used those files for Recommendation.

## Used Two Approaches
1. Natural Language Processing on Product Description
2. Convolutional Neural Network on Product Images

### Natural Language Processing (NLP) on Product Descriptions

**Approach Overview:**

In the NLP approach, we employ Natural Language Processing techniques to analyze and extract meaningful information from product descriptions. This textual analysis helps us understand the content and context of apparel items, enabling us to make better recommendations.

**Key Steps and Components:**

1. **Text Preprocessing:** This step involves cleaning and preparing the text data for analysis. Common tasks include:
   - Tokenization: Breaking text into individual words or tokens.
   - Stop-word Removal: Removing common words (e.g., "the," "and") that don't carry significant meaning.
   - Text Cleaning: Removing punctuation, special characters, and other noise from the text.

2. **Feature Extraction:** To represent text data in a numerical format suitable for machine learning models, we use techniques like:
   - TF-IDF (Term Frequency-Inverse Document Frequency): Assigning weights to words based on their frequency in the document and across documents.
   - Word Embeddings: Converting words into dense vector representations (e.g., Word2Vec, GloVe).

3. **Machine Learning Models:** We apply machine learning algorithms to make recommendations based on the extracted text features. Common models include:
   - Content-Based Filtering: Recommending items similar to those a user has shown interest in, based on product descriptions.
   - Collaborative Filtering: Recommending items based on user behavior and preferences, combined with text-based features.


### Convolutional Neural Network (CNN) on Product Images

**Approach Overview:**

In the CNN approach, we use Convolutional Neural Networks to analyze and extract features from product images. By processing the visual content of apparel items, we enhance our recommendation system's accuracy and visual appeal.

**Key Steps and Components:**

1. **Image Preprocessing:** Image preprocessing is crucial for preparing images for CNN analysis. It may include:
   - Resizing: Ensuring all images have consistent dimensions.
   - Normalization: Scaling pixel values to a standard range.
   - Augmentation: Introducing variations to the dataset by applying transformations like rotation or flipping.

2. **CNN Architecture:** We design a CNN model specifically for image analysis. A typical CNN architecture consists of convolutional layers, pooling layers, fully connected layers, and activation functions. These layers help extract hierarchical features from images.

3. **Training and Fine-Tuning:** The CNN model is trained on a labeled dataset of product images. During training, the model learns to recognize patterns and features in the images. Fine-tuning may involve adjusting hyperparameters and using techniques like transfer learning (e.g., using pre-trained models like VGG, ResNet) to improve performance.

4. **Integration with NLP:** In some cases, the features extracted from images are combined with features from the NLP approach to provide holistic recommendations. This fusion of visual and textual information enhances the recommendation quality.
