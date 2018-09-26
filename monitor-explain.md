---

copyright:
  years: 2018
lastupdated: "2018-9-26"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:tip: .tip}
{:pre: .pre}
{:codeblock: .codeblock}
{:screen: .screen}

# Explainability
{: #monitor-explain}

Explainability shows you the underlying factors that influenced the outcome of an individual transaction.
{: shortdesc}

## Configuring the Explainability monitor
{: #config-explain}

1.  From the *What is Explainability?* page, click **Next** to start the configuration process.

    ![What is Explainability? page](images/explain-what-is.png)

1.  On the *Specify type of input* page, select the type of data the deployment analyzes, for example: Numeric/categorical (structured data), Unstructured (text), or images.

    **Note**: Please note that for models that accept images as input, the image needs to be represented as a (height) x (width) x (# channels) format, where each point represents either monochrome or RGB values for each pixel. For models that accept text as input, it is expected that the model accepts the entire text, and not a vectorized representation of the text.

    ![Specify input type](images/explain-set-input.png)

    **Note**: Only classification models and python functions which have categorical output are supported. Regression models are not supported.

    Click **Next** to continue.

1.  Select the columns used to train the model - these are the features that your model deployment expects in a request. Click **Next**.

    ![Select column label](images/explain-select-column.png)

1.  Finally, select the columns that contained text, and have been converted to integers. For example, if the original training data contained `Male` and `Female` for *Gender*, and they have now been mapped to `0` and `1` respectively, the training data now contains `0` and `1` values for the *Gender* column. Identify such columns which now contain integers, but originally contained text values.

     ![Select data table](images/explain-text-column.png)

1.  Click the **Next** button.

    A summary of your selections is presented for review. If you want to change anything, click the **Edit** link for that section.

 Click **Save** to complete your configuration.

### Next steps
{: #explain-next}

From the *Configure monitors* page, you can select another monitoring category.
