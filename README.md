# Digitizing the Bookshelf - Số hóa tủ sách
This project focuses on automatically extracting key information from Vietnamese book cover images using computer vision and OCR techniques. The goal is to streamline the process of cataloging books by replacing manual data entry with an automated pipeline.

## Project Overview
- **Input**: Book cover images taken manually with mobile devices.
- **Output**: Extracted metadata including Title, Author, Publisher, and Other content.
- **Key Tasks**:
  1. Text Detection – Detect text regions using YOLOv8.
  2. Text Recognition – Extract text content using a fine-tuned VietOCR model.
  3. Information Synthesis – Organize recognized text into structured fields.
 
## Dataset
[Vietnamese Book Cover](https://www.kaggle.com/datasets/chithinguyen/vietnamese-book-covers)
- **Total images**: 964 book covers (manually collected).
- **Devices used**: iPhone, Samsung, iPad (to ensure variation).
- **Labeling tool**: PPOCRLabel
- **Annotation types**: Line-level bounding boxes with labels (title, author, publisher, other).
- **Split**: Train (700), Validation (132), Test (132)

##  Technologies Used
- **YOLOv8** – Object detection for text regions.
- **VietOCR** – OCR tailored for Vietnamese language.
- **Python, OpenCV, PyTorch**
- **PPOCRLabel** – For text region annotation

## Pipeline
```
Book Cover Image
       ↓
 [YOLOv8]
 Text Region Detection
       ↓
 [VietOCR]
 Text Recognition
       ↓
Information Synthesis
Structured Metadata (Title, Author, Publisher, Other)
```
## Lecturers:
  - TS. Lê Đình Duy
  - ThS. Phạm Nguyễn Trường An
## Members:
	- Bùi Lê Trọng Đức
	- Nguyễn Tiến Thịnh
	- Nguyễn Chí Thi


