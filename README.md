# codecademy_html

## Intro

### Project 01: Fashion Blog

Your friend Isa is a budding fashion blogger, and she’s asked you to build her a new website, just in time for New York Fashion Week!

## Tables

### Project 02: Wine Festival

In this project, we’re going to practice tabular organization in HTML so you can hone your skills and feel confident taking them to the real world. Why? If you’re going to have data on a webpage, you’ve got to master the skill of effectively and aesthetically organizing it – an HTML table is the perfect solution.

## Multimedia

### Project 03: NYC Blog

Create a blog about New York City using various semantic elements to show off how amazing the Big Apple is!

## Forms

### Project 04: Burger Menu

### Project 05: Login Validation

https://www.codecademy.com/courses/learn-html-forms/lessons/html-form-validation/exercises/validation-intro

### Project 06: Generate a Madlibs Story

https://www.codecademy.com/courses/learn-html-forms/projects/form-a-story

## CSS

project_07_SELECTORS_healthy_recipes
project_08_SELECTORS_olivia_woodruff_portfolio
project_09_BOX_davies_brugers 
project_10_POSITIONING_broadway                 
project_11_off-platform_dashmoto  
project_12_colors 
project_13_typology
project_14_BUTTONS_the_summit
project_15_BREADCRUMBS_blueberries
project_16_Style_Guide
project_17_Flexbox_to-do
project_18_FLEXBOX-tea_shop
project_19_Responsive_Design-Tsunami_Coffee

# Host on EC2 with Amazon Linux 2023

1. SSH into the instance

`ssh -i ~/keys/YOUR_KEY.pem ec2-user@YOUR_PUBLIC_IP`

2. Update system packages

`sudo dnf update -y`

3. Install nginx 

`sudo dnf install -y nginx`

4. Start and enable nginx

`sudo systemctl start nginx
sudo systemctl enable nginx`

5. Confirm it's running:

`systemctl status nginx`

6. Copy your HTML & CSS into nginx’s web root

`sudo cp -r ~/site/* /usr/share/nginx/html/`

7. Update permissions

`sudo chown -R nginx:nginx /usr/share/nginx/html`

8. Allow HTTP traffic in AWS Security Group

| Type | Protocol | Port | Source                        |
| ---- | -------- | ---- | ----------------------------- |
| HTTP | TCP      | 80   | 0.0.0.0/0 (and ::/0 for IPv6) |

9. Open your browser and visit

`http://YOUR_PUBLIC_IP/`