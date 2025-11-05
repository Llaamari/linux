![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Apache](https://img.shields.io/badge/apache-%23D42029.svg?style=for-the-badge&logo=apache&logoColor=white)<br>
cPouta Linux-VPS & Apache Assignment

This repository contains the implementation of a task requiring deployment of a Linux-based VPS in CSC cPouta, installation of an Apache web server, and hosting of a static HTML page over HTTP (port 80). The page has been personalized, and the service is configured to remain running.

⭐️ Assignment Requirements

| Requirement | Completed |
|-----------|-----------|
| Linux VPS in CSC cPouta | ✔️ |
| Apache installed and running | ✔️ |
| Static HTML page served over HTTP | ✔️ |
| Port 80 opened to the public | ✔️ |
| Service configured to stay active | ✔️ |
| Personalized webpage (not default Apache page) | ✔️ |
| No personal identifiers displayed | ✔️ |

⭐️ Implementation<br>
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) 

💡 Technologies Used
- Ubuntu Linux VPS (CSC cPouta)
- Apache2
- Static files (HTML, CSS, image)

💡 Repository Contents
- index.html
- style.css
- linux_cat.jpg

The 'index.html' file renders a personalized static welcome page using the stylesheet 'style.css' and the image 'linux_cat.jpg'.

⭐️ Server Configuration Summary

1. Install Apache (bash, sudo apt update, sudo apt install apache2)
2. Deploy web content:
  sudo cp index.html /var/www/html/
  sudo cp style.css /var/www/html/
  sudo cp linux_cat.jpg /var/www/html/
3. Ensure service stays running:
  sudo systemctl enable apache2
  sudo systemctl start apache2
4. Security groups in cPouta configured to allow inbound TCP traffic on port 80.

Project URL<br>
http://86.50.21.122/
