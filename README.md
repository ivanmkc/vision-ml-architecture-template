# vision-ml-architecture-template
## 1. Data ingestion and labelling pipeline

This uses:
- Google Cloud Storage: Stores unlabeled image files
- Google Cloud Pub/Sub: Detect changes to source image files
- Google Vertex AI -- DataLabelingJob: Creating a job
- Google Cloud Storage: Stores labeled image files and labels

## 2. 
# a. Training pipeline (Python script)

This uses:
- Google Cloud Pub/Sub: Detect changes to labeled image files
- Google Dataflow: Transform images (to augment dataset)
- Google Vertex AI -- Managed datasets
- Google Vertex AI -- Custom Training, AutoML
- Google Vertex AI -- Managed models
- Google Vertex AI -- Prediction
- Google Vertex AI -- Model export
- Optional: Google Vertex AI -- Model monitoring
- Optional: Google Vertex AI -- Feature Store

# b. Training pipeline (KFP)
Same as a) but using KubeflowPipelines

## User journeys
### Data ingestion
### Data transformation
### Model training
### Model prediction
### Orchestration