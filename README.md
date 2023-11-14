



# **FashionViz**: AI-Driven Fashion Recommendation Platform

![Alt text for your image](https://github.com/serbinaekaterinai/AI-Driven-Platform/blob/main/Images/Screenshot%202023-11-08%20at%207.35.58%20PM.png)

FashionViz is an innovative platform that integrates AI-driven fashion recommendations, immersive shopping experiences, and cutting-edge technologies such as Augmented Reality (AR) into the e-commerce landscape. This repository and documentation provide insights into the various aspects, methodologies, and technologies leveraged by FashionViz to enhance customer engagement and drive sales within the fashion retail industry.

This platform is designed to revolutionize the way customers interact with and purchase fashion products online. With the surge in online shopping and the growing potential of the global e-commerce market, FashionViz aims to provide a highly personalized and immersive shopping experience to meet the evolving demands of modern consumers.

## Industry Insights and Technological Integration in E-commerce
FashionViz operates within a dynamic industry heavily influenced by evolving market trends and changing consumer behaviors. Globally, the sales of clothing, footwear, and accessories have showcased steady growth, notably reaching $204.9 billion in the US market in the previous year. This sector has witnessed a significant shift towards online shopping, with 27% of consumers engaging in e-commerce, and a remarkable 76% making cross-border purchases. Moreover, a growing interest among US millennials (63%) in utilizing Augmented Reality (AR) to customize clothing items showcases a trend toward immersive and personalized experiences.

In response to these market dynamics, FashionViz strategically integrates technologies such as Augmented Reality (AR) and AI-driven recommendations to address the challenges of enhancing customer engagement and driving sales within the highly competitive e-commerce landscape.

This convergence of technology and consumer-driven experiences offers substantial opportunities for tech firms, retailers, and brands to enhance their market presence and engagement. FashionViz's innovative approach involves various stakeholders, including tech firms seeking innovation, fashion retailers and brands striving to enhance customer engagement and sales, as well as consumers seeking immersive and personalized shopping experiences in the e-commerce space.


## Data Overview

The dataset utilized by FashionViz is sourced from Kaggle.com and comprises two main components: a CSV file containing mapping details for various products within the fashion dataset, and an image folder housing over 44.4k high-resolution images (2400x1600) of fashion products.

## Recommendation System Development

FashionViz employs advanced recommendation systems to enhance user experience. Our first task was to predict gender, followed by predicting seasons, and finally, categorizing fashion items into various categories.

## Gender Binary Classification Analysis

The analysis of the dataset's gender classification revealed an inherent imbalance, prompting the decision to streamline the classification task solely to the 'Men' and 'Women' categories. The dataset presented a diverse range of gender labels, including 'Men,' 'Women,' 'Unisex,' 'Boys,' and 'Girls.' Due to this disparity and to simplify the classification process, the decision was made to concentrate specifically on the binary classification of 'Men' and 'Women'.

![Alt text for your image](https://github.com/serbinaekaterinai/Final-Project/blob/main/Images/Screenshot%202023-11-07%20at%208.24.31%20PM.png)



This strategic choice allowed for a more focused and efficient classification approach, addressing the imbalance in the dataset and streamlining the gender classification process to enhance the model's accuracy and effectiveness in discerning between male and female fashion items.

### Machine Learning Models and Model Performance

FashionViz implemented a variety of machine learning models for image classification within the realm of fashion. These models included Convolutional Neural Networks (CNN), Transfer Learning, ResNet50, and EfficientNetB3, each offering unique advantages for tackling image classification tasks.

- **Convolutional Neural Networks (CNN)**: CNNs, a foundational choice for image recognition, performed well in classifying fashion items. They demonstrated significant accuracy, although they were surpassed by other models in terms of performance.

- **Transfer Learning**: The utilization of transfer learning, where knowledge from one domain is applied to another, significantly improved accuracy. This approach proved effective, especially when dealing with limited fashion dataset. It exhibited a rapid learning curve and commendable performance.

- **ResNet50**: ResNet50, known for its depth and resilience against the vanishing gradient problem, exhibited robust performance. It excelled in handling deeper networks and achieved high accuracy and reliability in fashion item classification.

- **EfficientNetB3**: Among the models employed, EfficientNetB3 stood out as a top performer. The EfficientNet family's balanced scaling of network depth, width, and resolution resulted in exceptional accuracy. The model achieved approximately 98.20% accuracy on the validation dataset and consistently improved through fine-tuning, culminating in near-perfect accuracy on the test data.

![Alt text for your image](https://github.com/serbinaekaterinai/Final-Project/blob/main/Images/Screenshot%202023-11-07%20at%208.58.32%20PM.png)

### Model Performance Summary

In conclusion, the implementation of various machine learning models in FashionViz demonstrated their unique strengths and capabilities for image classification in the fashion industry. While all models delivered respectable results, EfficientNetB3, with hyper-tuning and its balanced scaling, emerged as the standout performer.

EfficientNetB3 showcased remarkable accuracy and efficiency, making it the model of choice for achieving near-optimal performance in the classification of fashion items. Its ability to learn intricate features, combined with the advantages of hyper-tuning, established EfficientNetB3 as the best-performing model in the FashionViz project.

## Seasonal Multiclass Classification Analysis

In addition to the gender binary classification analysis, FashionViz delved into a multiclass classification task specifically concerning the seasonal categorization of fashion items. The 'Season' column within the dataset presented an unbalanced distribution across different seasons, with a breakdown as follows:

![Alt text for your image](https://github.com/serbinaekaterinai/Final-Project/blob/main/Images/Screenshot%202023-11-07%20at%208.24.56%20PM.png)

While encountering this imbalance in the seasonal labels, a strategic decision was made to proceed with a multiclass classification approach, considering all the seasonal categories. To address the imbalance within the dataset, the employed technique involved the use of an ImageDataGenerator to augment the data. This augmentation process involved various transformations such as rotation, width and height shifting, shearing, zooming, horizontal flipping, and fill mode adjustments to create a more balanced representation of the different seasonal categories within the dataset.

Furthermore, class weights were calculated based on the distribution of labels in the seasonal dataset. This method helped account for the imbalance in the data by assigning different weights to each class, ensuring that the model learned effectively and made accurate predictions across all seasonal categories.

The use of such techniques aimed to balance the representation of seasonal categories, enabling the model to learn from a more diverse and augmented dataset, ultimately enhancing its ability to classify fashion items across various seasons effectively.

## Multi-Class Women's Fashion Essentials

In our analysis of fashion categories, we leveraged insights from Wunderlabel.com, revealing that certain items are particularly popular among women. Handbags, Tops, Heels, and T-shirts emerged as highly sought-after categories, supported by statistical data showcasing women's frequent purchases in these areas. 

This strategic decision to focus on these categories was reinforced by their balanced distribution, providing an ideal foundation for effective modeling and strategic decision-making. 
![Alt text for your image](https://github.com/serbinaekaterinai/AI-Driven-Platform/blob/main/Images/Screenshot%202023-11-13%20at%209.07.52%20AM.png)


Our experimentation encompassed various models, including CNN, MobileNet, and ResNet 50. Notably, The VGG16 model demonstrated exceptional performance, achieving close to 100% accuracy on both training and test sets. Impressively, this model exhibited efficiency, requiring only 8 minutes per epoch, showcasing a harmonious blend of speed and accuracy. 
![Alt text for your image](https://github.com/serbinaekaterinai/AI-Driven-Platform/blob/main/Images/Screenshot%202023-11-13%20at%208.53.26%20AM.png)

This comprehensive approach underscores our commitment to data-driven decision-making and the pursuit of optimal results in the realm of women's fashion essentials.

## Project Summary and Strategic Outlook

FashionViz's journey involved a comprehensive exploration and utilization of machine learning models for various classification tasks within the fashion dataset. The analysis encompassed both gender and seasonal multiclass classification, with strategic decisions made to handle the inherent imbalances within the dataset. For gender classification, a shift towards a binary approach focusing solely on 'Men' and 'Women' categories allowed for a more streamlined and efficient classification process. Similarly, in the seasonal multiclass classification, despite an initial imbalance, the utilization of augmentation techniques and calculated class weights facilitated a more balanced representation of different seasonal categories. Among the models employed, EfficientNetB3 emerged as a top performer, showcasing remarkable accuracy and efficiency.

### Business Recommendations and Future Work

Moving forward, there are several strategic recommendations and future areas of exploration for FashionViz:

1. **Advanced Model Development:** Explore building more complex and specialized models for fashion item classification, leveraging the success of EfficientNetB3 as a starting point to further refine and enhance model performance.

2. **Augmented Reality (AR) Application:** Consider developing an AR application for fashion e-commerce. This initiative could provide customers with a highly immersive shopping experience, allowing them to virtually try on products, visualize outfits, and receive personalized recommendations.

3. **Enhanced Data Collection:** Continuously improve and expand the dataset by collecting a more diverse range of fashion items and their attributes. This will aid in enhancing model training and accuracy.

4. **Customer-Centric Tools:** Develop tools that offer personalized fashion recommendations and styling advice, catering to individual preferences and enhancing customer engagement.

5. **Collaboration and Partnerships:** Explore collaborations with fashion brands and retailers to integrate the FashionViz platform, offering a more interactive and personalized shopping experience to their customers.

6. **User-Friendly Interface:** Focus on developing an intuitive and user-friendly interface for both mobile and web platforms, ensuring a seamless and enjoyable shopping experience.

These recommendations and future work areas aim to propel FashionViz towards providing cutting-edge, personalized, and immersive solutions within the fashion e-commerce space, ultimately enhancing customer engagement, driving sales, and establishing a strong foothold in the industry.
