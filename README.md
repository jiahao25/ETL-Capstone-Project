# ETL-Capstone-Project
Methodology and code on how I extract and transformed data from various sources in capstone project

## Files:
- Jupyter Notebook files -> Code
- character_strokes.txt -> Stroke order/count dataset
- multigram.json -> Output file containing chinese phrase frequencies
- onegram.json -> Output file containing single character frequencies and stroke order

## Datasets used:
- character_strokes.txt
- Leiden Weibo corpus: http://lwc.daanvanesch.nl/frequentwords.php

## Project Demonstration:

The user can type strokes on the orange area using the 5 basic strokes. The program will provide a visual feedback of the strokes that the user types in the green area. The top ranked character predictions will appear in the blue area.
![](https://raw.githubusercontent.com/jiahao25/ETL-Capstone-Project/master/pictures/keyboard1.JPG)

After the user selects the desired character, a few phrase suggestions will be displayed in the blue area. In this example, 你们， 你好 is shown.
![](https://raw.githubusercontent.com/jiahao25/ETL-Capstone-Project/master/pictures/keyboard2.JPG)

## Methodology

My role in the team is to deal with **data collection, cleaning and transforming** the relevant data to a form that allows the keyboard program to display character and phrase predictions **fast and accurately**. Below, I will demonstrate the process I took for the prototype to achieve this.
