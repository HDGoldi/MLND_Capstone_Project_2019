# Capstone Project - ChessBoard Recognition

## Overview of Output Labeling

* Color
    * w = White
    * b = Black

* Type
    * e = Empty
    * p = pawn
    * n = knight
    * b = Bishop
    * r = Rook
    * q = Queen
    * k = King


## Example Usage

select Images to be predicted in `ChessMain.py`
Run `pyton ChessMain.py`

Output will look like the following example:

`Predicted chess board:
br|bn|bb|bq|br|bb|bn|br
bn|bp|bp|bp|bp|bp|bp|bp
es|es|es|es|es|es|es|es
es|es|es|es|es|es|es|es
es|es|es|es|es|es|es|es
es|es|es|es|es|es|es|es
wp|wp|wp|wp|wp|wp|wp|wp
wr|wn|wb|wq|wk|wb|wn|wr`

## Setup

Data is available here: https://www.kaggle.com/dcuomo56/chess-board-data

In order to run first install all dependencies listed in requirements.txt. Then call python ChessMain.py from a terminal window. ChessMain.py contains example code on how to use the various objects. 

Folder structure for project is as follows:
```
Capstone Project
│   README.md
│   requirements.txt
|	ChessMain.py
|	ChessBoardProcessor.py
|	ChessBoardGenerator.py
|	CNNModel.py    
└───data
│   │   M.npy
│   └───models
│   |    	color_model.weights.best.hdf5
│   |    	piece_model.weights.best.hdf5
│   └───color_data
│   |   └───test
|	|	|	└─── black
|	|	|	└─── white
|	|	|	└─── square
|	|	└─── training
|	|	|	└─── black
|	|	|	└─── white
|	|	|	└─── square
|	|	└─── valid
|	|		└─── black
|	|		└─── white
|	|		└─── square
|	└───piece_data
│   |   └───test
|	|	|	└─── bishop
|	|	|	└─── king
|	|	|	└─── knight
|	|	|	└─── pawn
|	|	|	└─── queen
|	|	|	└─── rook
|	|	|	└─── square
│   |   └───train
|	|	|	└─── bishop
|	|	|	└─── king
|	|	|	└─── knight
|	|	|	└─── pawn
|	|	|	└─── queen
|	|	|	└─── rook
|	|	|	└─── square
│   |   └───valid
|	|	|	└─── bishop
|	|	|	└─── king
|	|	|	└─── knight
|	|	|	└─── pawn
|	|	|	└─── queen
|	|	|	└─── rook
|	|	|	└─── square
|	└───board_photos
│   |   └───set1
│   |   └───set2
│   |   └───test
└───notebooks
    │   Capstone_Background_Work.ipynb
    │   Neural Network Baseline Color.ipynb
    │   Neural Netowrk Baseline.ipynb
    │   Neural Network Data Generator.ipynb
    │   Neural Network Data Generator Augmentation.ipynb
    │   Neural Network Data Generator Augmentation Color.ipynb
```
