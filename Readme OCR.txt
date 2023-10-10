# Business Card Data Extraction using EasyOCR (Optical Character Recognition)

## Introduction

In today's fast-paced business world, efficiently managing and organizing contact information is essential for successful networking and communication. With the advancements in digital tools and technologies, manually entering business card details into a database can be time-consuming and error-prone. To address these challenges, developers can harness the power of Optical Character Recognition (OCR) and databases to automate the extraction of relevant information from business cards and store it for easy access.

One potent OCR library for text extraction from images is EasyOCR. EasyOCR is an open-source Python library that employs deep learning models to accurately recognize and extract text from various languages. By integrating EasyOCR with a MySQL database, developers can streamline the process of capturing business card data and storing it in an organized and structured manner.

## Developer's Guide

### 1. Tools Installation

To get started, make sure you have the following tools installed:

- Virtual code
- Python 3.11.0 or higher
- MySQL

### 2. Required Libraries to Install

Use pip to install the necessary libraries:

```
pip install pandas easyocr numpy Pillow opencv-python-headless os re sqlalchemy mysql-connector-python streamlit
```

### 3. Importing Libraries

#### Image Scanning Library

```python
import easyocr  # Optical Character Recognition
import numpy as np
from PIL import Image, ImageDraw
import cv2
import os
import re
```

#### Data Frame Libraries

```python
import pandas as pd
```

#### Database Library

```python
import sqlalchemy
import mysql.connector
from sqlalchemy import create_engine, inspect
```

#### Dashboard Library

```python
import streamlit as st
```

### 4. ETL Process

#### a) Extract Data

Utilize the EasyOCR library to extract relevant information from business cards.

#### b) Process and Transform the Data

After extraction, process the data based on fields such as Company name, Card Holder, Designation, Mobile Number, Email, Website, Area, City, State, and Pincode, and convert it into a data frame.

#### c) Load Data

Store the transformed data in a MySQL database for easy access.

## User Guide

### Step 1. Data Collection Zone

1. Click the **'Browse Files'** button to select an image.

### Step 2. Data Upload

2. Click the **'Upload to MySQL DB'** button to upload the data to the MySQL database.

### Step 3. Modification Zone

3. In the **'Modification Zone,'** you can modify the information and delete previous data as needed.

