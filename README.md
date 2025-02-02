# ETL-Capstone-Project
Methodology and code on how I extract and transformed data from various sources in capstone project

## Problem statement
Our client's patients belong to a group of patients suffering from motor neural related diseases, as a result they could not move their limbs and body. They use an eye gazing device and type in the eye gazing device to communicate. The problem is that these patients only know how to converse in Chinese and the eye gazing device do not have the support for that. Our team has to create a software within the eye gazing device that could allow the patients to converse by typing Chinese strokes. The chinese strokes are based on the standards provided by the National Language Committee in China (PDF attached in this repo).

## Files:
- Jupyter Notebook files -> Code
- character_strokes.txt -> Stroke order/count dataset
- multigram.json -> Output file containing chinese phrase frequencies
- onegram.json -> Output file containing single character frequencies and stroke order

## Datasets used:
- character_strokes.txt (It contains the official stroke order/count of recognised Chinese characters)
- Leiden Weibo corpus: http://lwc.daanvanesch.nl/frequentwords.php (It contains the single character usage and phrase usage information in the Weibo corpus)

## Project Demonstration:

The user can type strokes on the orange area using the 5 basic strokes. The program will provide a visual feedback of the strokes that the user types in the green area. The top ranked character predictions will appear in the blue area.
![](https://raw.githubusercontent.com/jiahao25/ETL-Capstone-Project/master/pictures/keyboard1.JPG)

After the user selects the desired character, a few phrase suggestions will be displayed in the blue area. In this example, 你们， 你好 is shown.
![](https://raw.githubusercontent.com/jiahao25/ETL-Capstone-Project/master/pictures/keyboard2.JPG)

## Methodology

My role in the team is to deal with **data collection, cleaning and transforming** the relevant data to a form that allows the keyboard program to display character and phrase predictions **fast and accurately**. The diagram below, I will demonstrate the process I took for the prototype to achieve this.

![](https://github.com/jiahao25/ETL-Capstone-Project/blob/master/pictures/diagram.JPG?raw=true)
