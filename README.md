# BizCardX-Extracting-Business-Card-Data-with-OCR
Introduction
The manual entry of business card information into a database can be time-consuming and error-prone. To prevent these difficulties, programmers can automate the process of collecting useful information from business cards and storing it for quick access using databases and optical character recognition (OCR). EasyOCR is a potent OCR library that makes it easier to extract text from images. An open-source Python package called EasyOCR uses deep learning models to precisely identify and extract text from a variety of languages. Developers may speed up the process of capturing business card data and storing it in a structured and organized manner by connecting EasyOCR with a MySQL database.

1. Tools Install
   
* Virtual code.
* Jupyter notebook.
* Python 3.11.0 or higher.
* MySQL.
  
2. Requirement Libraries to Install

pip install pandas easyocr numpy Pillow opencv-python-headless os re sqlalchemy mysql-connector-python streamlit

3.Import Libraries

Scanning library
import easyocr # (Optical Character Recognition)
import numpy as np
from PIL
from PIL import Image, ImageDraw
import cv2
import os
import re
Data frame libraries
import pandas as pd
Database Library
import sqlalchemy
import mysql.connector
from sqlalchemy import create_engine, inspect
Dashboard library
import streamlit as st

4. E T L Process

a) Extract data
Extract relevant information from business cards by using the easyOCR library
b) Process and Transform the data
After the extraction process, process the extracted data based on Company name, Card Holder, Designation, Mobile Number, Email, Website, Area, City, State, and Pincode is converted into a data frame.
c) Load data
After the transformation process, the data is stored in the MySQL database.
