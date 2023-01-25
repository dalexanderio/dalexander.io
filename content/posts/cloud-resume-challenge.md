---
title: "Cloud Resume Challenge"
date: 2023-01-24T18:22:44-06:00
draft: false 
---

I first heard about the cloud resume challenge a few months ago while studying for the AWS SysOps Administrator certification. The premise is using several AWS services to create a resume website that practically demonstrates the skills needed for a cloud engineering job.

The basics of the challenge are:

-   The site is hosted as a S3 static website
-   CloudFront is used to provide a CDN as well as HTTPS
-   The website uses HTML and CSS in such a way as to create a pleasant design
-   The site has a visitor counter that uses a combination of Javascript and a DynamoDB backend that communicates through an AWS API gateway
-   Source control is used and checks are done for any Python code running Lambda functions to update your database
-   You incorporate some element of IaC for updating your website

 Finally, you post about what you have learned.

Pretty straightforward, right?

Well, my site is currently live at [https://www.dory.cloud/](https://www.dory.cloud/) with a distinct lack of a visitor counter!

Why am I writing about my failure? Well, It's the biggest lesson I learned from the challenge. The initial stages were straightforward and I was able to set up a website with a CloudFormation template and CloudFront/S3 within an hour. However, I encountered difficulty configuring CORS for the Javascript counter and was unable to resolve the issue. With an interview approaching in two days, I had to make a decision on how to proceed. Instead of spending all my time trying to fix the visitor counter, I chose to focus on completing the CSS and finalizing my resume. This decision allowed me to present a polished website and utilize the extra time to prepare for the interview, which turned out to be more valuable as I didn't even have the opportunity to present the website!

I got the job, and have a half finished website but I learned a valuable lesson: deliver high value early. Focus on your end goal, not just the task you're working on at the moment.

I intend to return to this project some day, but I think what I got out of it was much more valuable than pasting code from Stack Overflow.
