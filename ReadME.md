
It is a study of lungs images and telling whether the person is effected with corona or not effected.

In this we have only 151 images each in effected and not effected data


We built the model using CNN Algorithm


conclusion:

Underfit / overfit We observe that model is not overfitting, as validation loss is better than training. This is explained by dropout - as dropout is not included in prediction, model is having full potential and generally making better predictions. However, if we add additional neurons, layers or filters, model will start performing badly, therefore, we can make a conclusion that we don't have removable bias in the model.

Generalizability of the model is limited, since the train set size is only around 151 images. Additionally, it is possible to include images of other pneumonia-like ilnesses and see if it is possible to build a model that would distinguish them correctly. It may be that this task would be significantly harder and we would need to go with just two classes - healthy person and coronavirus/other ilness, as differentiating of pneumonia/coronavirus may be incredibly hard from just CT scans.

How to make better model - we can take pretrained model (or pretrain it by ourselves) that is capable of diagnosing similar illnesses and apply transfer learning with COVID-19 dataset. CT lungs scans of person with pneumonia can be quite close to CT scans of person with coronavirus, so, such dataset can be used.

Since we are not setting seed, performance may slightly vary, but accuracy is 100%. If we continue training, we observe overfitting, therefore we stop our training after 40 epochs