# LIB-ThermalPerception-Dataset

**Dataset**: LIBTPD_V1  
**Version**: v1.0  
**License**: Apache License 2.0  
**Contact**: huixin_xu@tju.edu.cn  

## 1) Overview:
LIB-ThermalPerception-Dataset (LIBTPD) is an ANSYS-simulated dataset of Li-ion battery thermal faults for training/fine-tuning vision models in automatic detection, tracking, and segmentation. It includes thermal images, binary masks, and box prompts, and supports common detectors and promptable Vision Foundation Models (VFMs).

## 2) Directory Structure
- LIBTPD_V1/
  - README.md               # Dataset description
  - LICENSE                 # Apache License 2.0
  - simulation/             # Simulated data
    - 1P1S/
    - 1P1S_3views/
    - 1P2S/
    - 1P3S/
  - processed_finetune/     # Pre-processed fine-tuning data
    - train/
      - images/             # Training images
      - boxes/              # JSON box prompts (same basename as images)
      - masks/              # Binary masks (0/255)
    - val/
      - images/             # Validation images
      - boxes/              # Validation box prompts
      - masks/              # Validation masks
    - test/
      - images/             # Test images
      - boxes/              # Test box prompts
      - masks/              # Test masks

## 3) Data Format:
- **Images**: 24-bit PNG format.
- **Masks**: Binary 24-bit PNG (0 = background, 255 = foreground), same name and size as the image.
- **Boxes (JSON)**: Pixel-coordinate box prompts, with the same basename as the images.

## 4) License:
The dataset is released under the **Apache License 2.0**.
