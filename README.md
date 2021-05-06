# NMT Attention Alignment Visualizations
An attention alignment visualization tool for command line and web. 

Model Checkpoints
https://drive.google.com/drive/folders/1wKR1BmSPeJJ567Qqroj72wLI6b5l1qtw?usp=sharing

Model SourceCode
https://colab.research.google.com/drive/1Sqlz1pHrNodGe8IkejAXtL8G3uba06e_?usp=sharing

Data set link
https://drive.google.com/drive/folders/1FBOZ6rXCeI6EVxC76Cj_B8Q3aOGd8lO4?usp=sharing

github repo link
https://github.com/TrushaSakharkar/NLP_Project

Usage
---------

  - Translate text and get word or subword level alignments using our model code
  - Visualize the alignments
    - in the command line standard output
    - in a web browser (PHP required)

Installation
---------

From the repository - this way you get all files including pregenerated alignments and the web version for viewing.
```bash
git clone https://github.com/TrushaSakharkar/NLP_Project.git
cd NLP_Project
python3 softalignments/process_alignments.py -i input/alignments.txt -o color/web
```

From the zip - this way you get all files including pregenerated alignments and the web version for viewing.
```bash
unzip filename.zip
cd NLP_Project
python3 softalignments/process_alignments.py -i input/alignments.txt -o color/web
```

Requirements
---------

* Python 3.6 or newer

    * NLTK for BLEU calculation(requires Python versions 3.5, 3.6, 3.7, or 3.8)
	
	* Numpy
	
	```bash
	pip3 install numpy nltk
	```

* PHP 5.4 or newer (for web visualization)

Examples
---------

  - in the command line as shaded blocks. 
	```sh
	python3 softalignments/process_alignments.py -i input/alignments.txt -o color
	```
	
	  or
	```sh
	python3 softalignments/process_alignments.py -i input/alignments.txt -o block2
	```
		
  - in the browser as links between words
	
	```sh
	python3 softalignments/process_alignments.py -i input/alignments.txt -o web
	```

Screenshots
---------
Color
![N|Solid](https://github.com/TrushaSakharkar/NLP_Project/blob/master/img/terminal.png)
 
<!-- ![N|Solid](https://github.com/M4t1ss/sAliViz/blob/master/assets/Screenshots/colorAlignments.PNG?raw=true) ![N|Solid](https://github.com/M4t1ss/sAliViz/blob/master/assets/Screenshots/blockAlignments.PNG?raw=true) ![N|Solid](https://github.com/M4t1ss/sAliViz/blob/master/assets/Screenshots/block2.png?raw=true)  -->

Web
<!-- ![N|Solid](https://github.com/M4t1ss/sAliViz/blob/master/assets/Screenshots/webAlignments.PNG?raw=true) -->
![N|Solid](https://github.com/TrushaSakharkar/NLP_Project/blob/master/img/edge.png)
![N|Solid](https://github.com/TrushaSakharkar/NLP_Project/blob/master/img/matrix.png)



