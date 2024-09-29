Deploy a static website using GitHub action and s3 bucket

- Create an ec2 instance
- Create a project repository and index.html

- Install git on EC2 instance : yum install git -y
- Add ssh-key of EC2 instance to github ssh-keys
- Create one empty github repository
- Upload main.yml in project-repo >> .github >> workflows >> main.yml

- Create s3 bucket
- Uncheck block public access
- Enable Static Website Hosting
- Add following permission policy

- Add AWS_SECRET_KEY and AWS_ACCESS_KEY in github_repo >> settings >> secret and variables >> actions >> new repository secret
- Add remote origin to the remote repo
- Commit and push code to the github repository
- Code will automatically push to s3 bucket
- Copy obejct URL of index.html and paste in Browser
