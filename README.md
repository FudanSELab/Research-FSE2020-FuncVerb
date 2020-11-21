#### Replication package for paper: API Method Recommendation via Explicit Matching of Functionality Verb Phrases

##### [Open Source Python Library](https://github.com/FudanSELab/funcverbnet)
We are building an open source python library, [funcverbnet](https://github.com/FudanSELab/funcverbnet), to provide data and easy-to-use interfaces to our data and analysis technologies. Any suggestions and feedback are welcome！！！Please！！！

##### Attention:

We call the functionality sentence  _f\_sentence_

A  _f\_sentence_ can be classiﬁed into a functionality category (or _f\_category_)

The _f\_sentence_ from a _f\_category_ share a set of phrase patterns (or _p\_pattern_)

We conducted an empirical study to understand what _f\_verbs_, _p\_pattern_,
and _f\_categories_ are present in API _f\_sentence_. Specifically,we focus
on answering the following research questions:

##### RQ1: What verbs are used in the API _f\_sentences_

1. [sorted_verb_count.txt](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/RQ1/sorted_verb_count.txt) shows the all verbs we collect from _f\_sentences_ of Java and Android API methods. There are 931 verbs including the verb "return", and 87 verbs(9.34%) of them appear in 80% _f\_sentences_. 930 verbs excluding the verb "return", and 115 verbs(12.37%) of them appear in 80% _f\_sentences_.
2. [verb_count.xlsx](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/RQ1/verb_count.xlsx) includes the appearance count in _f\_sentences_ of all 931 verbs. Each row contains four parts. The first part is the verb, the second is the appearance count of this verb, the third is the index, and the last part is the log result of the count. Also, there are four figures that show the trend of the verb count's change. 
3. Total _f\_sentences_ (54256). [total_functionality_descriptions.csv](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/RQ1/total_functionality_descriptions.csv) contains 54,256 _f\_sentences_ filtered from Java and Android API methods. Each piece of data contains API's qualified name and its _f\_sentence_.

##### RQ2: What _f\_categories_ can the _f\_sentences_ be classified into?

1. [functionality_category.tsv](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/RQ2/functionality_category.tsv) shows the _f\_categories_ we summarized. It mainly includes four parts. The first column shows the total verbs of each _f\_category_, the second column is the label verb of each _f\_category_, the third is the number of verbs that each _f\_category_ contains and the last column shows three example _f\_sentences_ of each _f\_category_.

   For example, the label verb of functionality category "cancel/deregister/undo/deny/unset/unschedule/unregister/unbind/uninitialize/unload/deselect/unlock/unblock" is "cancel", it contains 13 verbs. ['Cancels the speech recognition.', 'Instructs the WebView to cancel the authentication request.', 'Cancels the current editing session.'] are three example _f\_sentences_ of this category.

2. [annotation_website](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/RQ2/annotation_website.png) is a screenshot of our annotation website.

3. [1,139 f_sentences with annotation](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Annotation_data/1139_f_sentences_with_annotation.csv) for coding protocol definition phase.

4. [13,635 f_sentences with annotation](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Annotation_data/13635_f_sentences_with_annotation.csv) for coding protocol definition phase and annotation phase.

5. [14,774 f_sentences with annotation](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Annotation_data/14774_f_sentences_with_annotation.csv) for coding protocol definition phase and annotation phase. "single_description" is the sentences, "final_annotation_type" is a id representing the f_category. 


##### RQ3: What _p\_patterns_ are used in the _f\_sentences_ from each _f\_category_?

1. [p_pattern_for_category.txt](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/RQ3/p_pattern_for_category.txt) shows all _p\_patterns_ used in each _f\_category_.


##### Evaluation
1. [5-fold cross validation accuracy](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Evaluation/5_fold_cross_validation_accuracy.xlsx) shows the accuracy of each fold cross validation for category classification.


2. [poi_test_sentences](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Evaluation/POI_Data.xlsx) shows the data for _p\_patterns_ evaluation in poi. The first column is the sentences. The second and third column are annotation _f\_category_ and annotation _p\_pattern_. The fourth and fifth column are automatic _f\_category_ and automatic _p\_pattern_. The last two column represent if the automatic _f\_category_ and _p\_pattern_ are correct.

3. [evaluation_questions_with_answers.xlsx](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Evaluation/evaluation_questions_with_answers.xlsx) shows the task questions and answers. Also the group which the task belong to is in the file at column. [Task1.docx](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Evaluation/Task1.docx) shows a template which participants need to fill in. [Evaluation_Answer.xlsx](https://github.com/FudanSELab/Research-FSE2020-FuncVerb/blob/master/Evaluation/Evaluation_Answer.xlsx) shows the data that participants record in the tasks. the first column is the question's stackoverflow url. The second column is question title. The third column is the standard answer. 4~15th column represents if the participant find the correct answer via the tools. Next to them are the total and average number of participants who find the answer using the tools.

