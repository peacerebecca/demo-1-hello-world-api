1)Go to google artifact registry and enable the API

2) Create repository
	a. Name: my-docker-images-repo
	b. Format: Docker
	c. Location Type: Region

gcloud auth login
gcloud projects list
gcloud config set project <project_id>


6) Go to Cloud Source Repositories
    a. Create repo, follow instructions and push code
    b. Change Cloud build file with correct container registry repo name

git init
git add .
git commit -m 'initial checkin'
git remote add origin <url>
git push -u origin master

7) Go to Cloud Build and enable API and setup build trigger
    cloud build config file location: demo-1-hello-world-api/cloudbuild.yaml
    build

8) Go to Cloud Run and click on Setup Continuous Deployment

9) Change source file. commit and wait for the build to happen
