Segment Anything Model (SAM) implementation for my ML students

Platform: MacBook Air M1, 8GB, macOS Sonoma 14.6.1, Total Number of Cores: 8 (4 performance and 4 efficiency) Python Version 3.10.14 (running in Conda virtual environment) Jupyter Notebook

IMPORTS TO ENSURE AVAILABLE: 
import os import cv2 
import torch 
import roboflow 
import base64 
import supervision as sv 
import numpy as np 
from roboflow import Roboflow 
from fastsam import FastSAM, FastSAMPrompt 
from segment_anything import sam_model_registry, SamAutomaticMaskGenerator, SamPredictor 
from matplotlib.backends.backend_agg import FigureCanvasAgg


WEIGHTS REQUIRED INSIDE THE "WEIGHTS" FOLDER
Missing weights you need to download elsewhere: FastSAM-s.pt /FastSAM-x.pt /FastSAM.pt and weights/sam_vit_h_4b8939.pth
