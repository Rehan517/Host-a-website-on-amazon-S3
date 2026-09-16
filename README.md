<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://nextwork.ai/projects/aws-host-a-website-on-s3)

**Author:** Rehan Ali  
**Email:** rehan.ali.maq@gmail.com

---

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate how to host a website using amazon S3. I'm doing this project to learn how to use and implement amazon S3

### Tools and concepts

Services I used were amazon S3. Key concepts I learnt include uploading objects into a bucket and hosting a static website using static hosting

### Time, challenges, and wins

This project took me approximately 25-30 mins. The most challenging part was uploading the object. It was most rewarding to host the website and see the results

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will create a new bucket because files will be saved in this bucket

### How long it took to create the bucket

Creating an S3 bucket took me 3 mins

### Region selection

The Region I picked for my S3 bucket was ap-southeast-2 because this is the closest to my location

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means that the name for bucket has to be unique meaning no other bucket has that name as this is like unique url that will be used

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

In this step, I will setting up the website an uploading objects into the s3 bucket because it allows. to store many files

### Files I uploaded

I uploaded two files to my S3 bucket - they were index.html and the folder 

### How the files work together

Both files are necessary for this project as the index.html creates the page and the folder has the images and the styling for the page

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step, I will host the website and its content because it needs to be accessed by the public

### Understanding website hosting

Website hosting means publishing your website so that its public

### How I enabled website hosting

To enable website hosting with my S3 bucket, I went to the static website hosting settings  and enabled it

### Access Control Lists (ACLs)

An ACL is a set of rules that decides who can access the ACL and in this project i have enabled it

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is the public url the website can be accessed through

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw 403 forbidden The reason for this error was that the content in the bucket is still private evne tough the bucket itself is public

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I will make the bucket files public because it needs to be done to access the website

### How I resolved the 403 error

To resolve this 403 Forbidden error, I went into the bucket and make the objects by adding them into the ACL

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this project extension I'm about to adjust the bucket policies I'm doing this so that no one can delete index.html

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are ways to limit certain actions for the bucket. The benefit of using bucket policies is that they are more granular alowing further contrl while ACLs are useful for general changes

![Image](http://nextwork.ai/lighthearted_brown_silly_apricot/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy stops for the indx.html file being deleted. I tested this by trying to delete it and saw that it came up with an error

---

---
