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





