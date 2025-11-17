# cPouta Linux-VPS & Apache Assignment
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Apache](https://img.shields.io/badge/Apache-%23D42029.svg?style=for-the-badge&logo=apache&logoColor=white)

This repository contains the implementation of a task requiring deployment of a Linux-based VPS in CSC cPouta, installation of an Apache web server, and hosting of a static HTML page over HTTP (port 80). The page has been personalized, and the service is configured to remain running.

## Assignment Requirements

| Requirement | Completed |
|-----------|-----------|
| Linux VPS in CSC cPouta | ✔️ |
| Apache installed and running | ✔️ |
| Static HTML page served over HTTP | ✔️ |
| Port 80 opened to the public | ✔️ |
| Service configured to stay active | ✔️ |
| Personalized webpage (not default Apache page) | ✔️ |
| No personal identifiers displayed | ✔️ |

## Implementation

### Technologies Used
- Ubuntu Linux VPS (CSC cPouta)
- Apache2
- Static files (HTML, CSS, image)<br>
  ![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
  ![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

### Repository Contents
[index.html](https://github.com/Llaamari/linux/blob/main/index.html)<br>
[style.cssl](https://github.com/Llaamari/linux/blob/main/style.css)<br>
[linux_cat.jpg](https://github.com/Llaamari/linux/blob/main/linux_cat.jpg)<br>
The `index.html` file renders a personalized static welcome page using the stylesheet `style.css` and the image `linux_cat.jpg`.

## Server Configuration Summary

Install Apache:<br>
![Bash Script](https://img.shields.io/badge/Bash_Script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)
```bash
sudo apt update
sudo apt install apache2
sudo cp index.html /var/www/html/
sudo cp style.css /var/www/html/
sudo cp linux_cat.jpg /var/www/html/
sudo systemctl enable apache2
sudo systemctl start apache2
```
Security groups in cPouta configured to allow inbound TCP traffic on port 80.
