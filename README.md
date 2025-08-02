# devops-cicd-ec2
Sure! Here's a solid README template tailored for your Flask + Docker + DevOps project that you can customize:

---

# DevOps CICD EC2 - Flask Web App with Docker and CI/CD

## Overview

This project is a simple Flask web application containerized with Docker and set up with a CI/CD pipeline using GitHub Actions to deploy on AWS EC2.

It demonstrates:

* Building and running Flask apps with Docker
* Using Flask templates and static files for multi-page websites
* Automating build and deployment with GitHub Actions
* Deploying containerized apps to AWS EC2

---

## Project Structure

```
.
├── app.py                 # Flask app source code
├── Dockerfile             # Docker image definition
├── requirements.txt       # Python dependencies
├── templates/             # HTML templates for Flask
├── static/                # Static assets like CSS
├── .github/workflows/     # GitHub Actions CI/CD workflows
├── README.md              # Project documentation
└── LICENSE                # License details
```

---

## Setup & Run Locally

1. Clone the repo:

   ```bash
   git clone https://github.com/harishekar10/devops-cicd-ec2.git
   cd devops-cicd-ec2
   ```

2. Create and activate virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the app:

   ```bash
   python app.py
   ```

5. Open browser at [http://localhost:5000](http://localhost:5000)

---

## Build and Run with Docker

1. Build Docker image:

   ```bash
   docker build -t flask-webapp .
   ```

2. Run container:

   ```bash
   docker run -p 5000:5000 flask-webapp
   ```

3. Open browser at [http://localhost:5000](http://localhost:5000)

---

## CI/CD Pipeline

This project uses **GitHub Actions** to:

* Build Docker image on every push
* Push the image to Docker Hub (or any container registry you configure)
* Deploy the container on AWS EC2 instance

> ⚠Ensure your AWS credentials and Docker Hub credentials are configured as GitHub Secrets.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact

Feel free to reach out:

* Email: [harishekar10@gmail.com](mailto:harishekar10@gmail.com)
* GitHub: [harishekar10](https://github.com/harishekar10)

---

Would you like me to generate the full markdown file for you? Or help add badges (build status, license) and screenshots?

