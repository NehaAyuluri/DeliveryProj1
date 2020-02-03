# Continuous Delivery of Flask Application using GCP
1. Create Project in GCP 
2. Activate cloud shell by and verify if it is refering to your project created or not.
3. [Refer to] (https://cloud.google.com/appengine/docs/standard/python3/quickstart)
4. Run describe to verify if project is working. Output should have projectname, projectid and the project should be in ACTIVE state ```gcloud projects describe $GOOGLE_CLOUD_PROJECT```
5. If you want to change the project you can do using ```gcloud config set project $GOOGLE_CLOUD_PROJECT```
6. App Engine creation ```gcloud app create ``` If prompted for region select us-central
7. Clone the hello world sample app repo using ```git clone https://github.com/GoogleCloudPlatform/python-docs-samples```
8. cd into the repo ```cd python-docs-samples/appengine/standard_python37/hello_world```
9. Creating the virtual env ```virtualenv --python $(which python3) ~/.YOUR PROJECT NAME```
10. Sourcing the virtual env ```source ~/.YOUR PROJECT NAME/bin/activate```
11. Activate cloud shell editor and run flask locally ```python main.py```
12. App can be previewed using web preview on top right corner of the shell
13. Update main.py for different routes
14. You can deploy the app using ```gcloud app deploy```
15. [Deployments with cloud build can learned through this link] (https://cloud.google.com/source-repositories/docs/quickstart-triggering-builds-with-source-repositories)