# daily-dialogs-dataset

https://huggingface.co/datasets/li2017dailydialog/daily_dialog


## Dataset Summary

High-quality multi-turn dialog dataset, DailyDialog, which is intriguing in several aspects. The language is human-written and less noisy. The dialogues in the dataset reflect our daily communication way and cover various topics about our daily life. We also manually label the developed dataset with communication intention and emotion information. Then, we evaluate existing approaches on DailyDialog dataset and hope it benefit the research field of dialog systems.


### Metadata

```
annotations_creators:
  - expert-generated
language_creators:
  - found
language:
  - en
license:
  - cc-by-nc-sa-4.0
multilinguality:
  - monolingual
size_categories:
  - 10K<n<100K
source_datasets:
  - original
task_categories:
  - text-classification
task_ids:
  - multi-label-classification
paperswithcode_id: dailydialog
pretty_name: DailyDialog
tags:
  - emotion-classification
  - dialog-act-classification
dataset_info:
  features:
    - name: dialog
      sequence: string
    - name: act
      sequence:
        class_label:
          names:
            '0': __dummy__
            '1': inform
            '2': question
            '3': directive
            '4': commissive
    - name: emotion
      sequence:
        class_label:
          names:
            '0': no emotion
            '1': anger
            '2': disgust
            '3': fear
            '4': happiness
            '5': sadness
            '6': surprise
  splits:
    - name: train
      num_bytes: 7296715
      num_examples: 11118
    - name: test
      num_bytes: 655844
      num_examples: 1000
    - name: validation
      num_bytes: 673943
      num_examples: 1000
  download_size: 4475921
  dataset_size: 8626502
  ```

### This example was too long and was cropped:

```
{
    "act": [2, 1, 1, 1, 1, 2, 3, 2, 3, 4],
    "dialog": "[\"Good afternoon . This is Michelle Li speaking , calling on behalf of IBA . Is Mr Meng available at all ? \", \" This is Mr Meng ...",
    "emotion": [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
}
```

### Licensing Information


DailyDialog dataset is licensed under (CC BY-NC-SA 4.0)[https://creativecommons.org/licenses/by-nc-sa/4.0/].


### Citation Information

```
@InProceedings{li2017dailydialog,
    author = {Li, Yanran and Su, Hui and Shen, Xiaoyu and Li, Wenjie and Cao, Ziqiang and Niu, Shuzi},
    title = {DailyDialog: A Manually Labelled Multi-turn Dialogue Dataset},
    booktitle = {Proceedings of The 8th International Joint Conference on Natural Language Processing (IJCNLP 2017)},
    year = {2017}
}
```