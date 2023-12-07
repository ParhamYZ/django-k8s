# django-k8s
This is a project to practice kubernetes by deploying a django app.

The purpose of this project is making a connection between django app and postgresql on kubernetes clusters. 

At first, a docker compose is used to verify creation of django app image via Dockerfile, configurations of django app and postgresql db and finally communications of app and db such as migrating and creating superuser.

Then, some examples is practiced with kubernetes such as deploying nginx and a fastAPI app.

After that, the django app is deployed on kubernetes on Digital Ocean servers in these steps:

- The cluster is defined on Digital Ocean kubernetes section.
- The django app image is created and pushed to Digital Ocean container registry section.
- The postgresql DB is defined on Digital Ocean databases section.
- The deployments, services and secrets are defined on kubernetes.

Finally, for manual deployment guideline on github, a documentaion is provided as "deployment-guide.md" but there is some yaml file in ".github" folder that defines github actions steps. 

It was a great experience on practicing and understanding kubernetes concepts thanks to Coding For Entrepreneurs.
You can watch the full tutorial on this link:
https://youtu.be/NAOsLaB6Lfc?si=MTXw43WURV5_CFAo
