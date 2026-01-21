# NelloreBeefCattleDataset

Nellore cattle dataset

<img width="2048" height="1384" alt="fig1" src="https://github.com/user-attachments/assets/b32c0c5e-be35-4e7f-8c7b-825e03646ba3" />

# Image acquisition

A field study was carried out at the Fazenda Campanário feedlot in Laguna Carapã, Mato Grosso do Sul, Brazil (22°47'8" S; 55°3'57" W), which houses approximately 14,600 cattle. Data acquisition was performed using a multirotor UAV (DJI Phantom 4 Advanced) equipped with a 20-megapixel Sony camera (4864 × 3648 pixels). \textcolor{blue}{All flights were conducted at a fixed altitude of 15m to maintain consistent spatial resolution. Twelve flight operations were carried out at approximately 10-day intervals. Image acquisition was performed using a 90 degree camera angle, with a 70\% overlap between consecutive images. Data collection was conducted in the morning, between 7:00 and 9:00 a.m., under varying weather conditions, including cloudy, sunny and rainy scenarios. The acquisition platform operated at a speed of 10 km/h.} \textcolor{blue}{Monitoring was performed over a 112-day period, starting on July 10, 2024 (Fig.~\ref{fig:uav_setup}). The average age of the cattle at the beginning of the feedlot period was 18 months.}

(A) Aerial view of the feedlot at Fazenda Campanário; (B) UAV operation at approximately 15m altitude; (C) representative top-view images acquired during the flights; (D) and (E) enlarged images.

All collected images were subjected to a systematic cleaning process to optimize data quality prior to model development. Frames without cattle, images showing excessive overlap between individuals, and scenes dominated by vegetation or empty ground were removed. After filtering, 954 high-quality images remained \textcolor{blue}{in total for this study}. \textcolor{blue}{From this pool, 370 images were randomly selected and manually annotated with bounding boxes covering the full body extent of each visible animal. These annotated samples were used to fine-tune the YOLOv11s detector, whereas the remaining unannotated images were reserved for automatic inference using the fine-tuned model, thereby substantially reducing the manual labeling workload.

Manual bounding box annotations were performed on these images. Each visible animal in the training set was labeled with a bounding box covering the entire body extent. The annotated dataset was then \textcolor{blue}{randomly} split into training (80\%), validation (10\%), and test (10\%) subsets using stratified sampling to preserve representative variability in individual animals and imaging conditions. \textcolor{blue}{The training and validation subsets were used during the training process for model optimization and hyperparameter tuning, whereas the test subset was held out throughout training and employed exclusively for the final performance evaluation.

# Dataset download 

Link: http://evertontetila.ws.ufgd.edu.br/Datasets/NelloreBeefCattleDataset.zip

