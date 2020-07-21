<h1 class="code-line" data-line-start=0 data-line-end=1 ><a id="FIT5149_S1_2020_Assessment_2_Authorship_Profiling_0"></a>FIT5149 S1 2020 Assessment 2: Authorship Profiling</h1>
<h2 class="code-line" data-line-start=2 data-line-end=3 ><a id="Description_2"></a>Description</h2>
<p class="has-line-data" data-line-start="4" data-line-end="5">These files generate the preprocessing and modelling for gender classification of tweets for an internal Monash Kaggle competition. The best model we were able to train was the Logistic Regression in <code>group41_ass2_final_classifier.ipynb</code>.</p>
<h2 class="code-line" data-line-start=6 data-line-end=7 ><a id="Files_6"></a>Files</h2>
<p class="has-line-data" data-line-start="8" data-line-end="9">This project comprises two Python3 Jupyter Notebook files:</p>
<ol>
<li class="has-line-data" data-line-start="10" data-line-end="11">group41_ass2_wrangling.ipynb</li>
<li class="has-line-data" data-line-start="11" data-line-end="13">group41_ass2_final_classifier.ipynb</li>
</ol>
<p class="has-line-data" data-line-start="13" data-line-end="14">Two .csv:</p>
<ol start="3">
<li class="has-line-data" data-line-start="15" data-line-end="16">train_labels.csv</li>
<li class="has-line-data" data-line-start="16" data-line-end="17">test_labels.csv</li>
</ol>
<p class="has-line-data" data-line-start="18" data-line-end="18">Two .npy:</p>
<ol start="4">
<li class="has-line-data" data-line-start="20" data-line-end="20">bw_train.npy</li>
<li class="has-line-data" data-line-start="21" data-line-end="21">bw_test.npy</li>
<li class="has-line-data" data-line-start="22" data-line-end="22">test_index_list.npy</li>
</ol>
<h2 class="code-line" data-line-start=25 data-line-end=26 ><a id="Usage_24"></a>Usage</h2>
<h3 class="code-line" data-line-start=26 data-line-end=27 ><a id="Logistic_Regression_Test_Predictions_25"></a>Logistic Regression Test Predictions</h3>
<p class="has-line-data" data-line-start="28" data-line-end="29">To simply generate the final <code>pred labels.csv</code>, where the label prediction on the testing documents is stored, you can run the <code>group41_ass2_final_classifier.ipynb</code> file, which will be using <code>train_labels.csv</code>, <code>bw_train.npy</code>, <code>bw_test.npy</code> and <code>test_index_list.npy</code> to train and test the best selected model (Logistic Regression).</p>
<h3 class="code-line" data-line-start=30 data-line-end=31 ><a id="Data_Preparation__Feature_Extration_29"></a>Data Preparation &amp; Feature Extration</h3>
<p class="has-line-data" data-line-start="32" data-line-end="33">To analyse the pre-processing steps, please open <code>group41_ass2_wrangling.ipynb</code>. It will go the data reading, preparation and feature extraction. The final method used for the modelling part was “CountVectorizer” with words and characters n-grams model. This is what generates <code>bw_train.npy</code> and <code>bw_test.npy</code>, which are the necessary files to run the top selected model. In order to run this file from the scratch, you need to add the <code>data</code> folder containing the unzipped <code>data.zip</code> contents in the same folder as you have the codes.</p>