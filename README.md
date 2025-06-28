# Personal Portfolio Website

A modern, personal portfolio website built with React, TypeScript, Tailwind CSS, shadcn/ui, and powered by a serverless AWS backend.  
Visitors can easily contact me using a secure form, which sends email notifications using AWS Lambda, SES, and API Gateway.

---

## 🚀 Tech Stack

- **Vite** – Build tool for rapid development and hot module replacement  
- **React** (with TypeScript) – UI development with strong typing  
- **Tailwind CSS** – Utility-first CSS for fast, responsive design  
- **shadcn/ui** – Accessible, reusable React UI components  
- **React Router** – Seamless client-side routing  
- **Lucide React** – Modern icon set for React apps  

---

## ☁️ Cloud Hosting & Serverless Architecture

- **AWS S3** – Static website hosting  
- **AWS CloudFront** – CDN for global content delivery and SSL termination  
- **AWS API Gateway** – Secure REST API endpoint for the contact form  
- **AWS Lambda** – Serverless backend for handling contact submissions  
- **Amazon SES** – Transactional email delivery (notifies me & confirms to user)  
- **Amazon Route 53** – DNS management with custom domain routing  
- **AWS Certificate Manager** – Free SSL certificates integrated with CloudFront  

---

## 🔁 CI/CD with GitHub Actions

This project uses a GitHub Actions CI/CD pipeline to automate deployment to AWS.  
Every time changes are pushed to the `main` branch, the site is rebuilt, deployed to S3, and CloudFront cache is invalidated — ensuring a seamless update process.

---

## 📫 Contact Form Flow

1. User submits the contact form.  
2. **API Gateway** receives the POST request.  
3. **Lambda** function processes the submission.  
4. **SES** sends:  
   - A notification email to my inbox  
   - An automatic thank-you/confirmation email to the user  

---

## 🛠️ Local Development

```bash
# Install dependencies
npm install

# Run local development server
npm run dev

# Build for production
npm run build
```
## 🌐 Live Site
https://ceeeentd.cv
