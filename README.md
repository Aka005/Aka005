# 😸 Hey, I'm Emily Jao!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Emily%20Jao-blue?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/emily-jao-wb01/)  [![GitHub](https://img.shields.io/badge/GitHub-Aka005-black?logo=github&logoColor=white)](https://github.com/Aka005)

About Me: 
**Important:**  

I’m a junior at **The Pennsylvania State University**, majoring in **Cybersecurity** with a minor in **Information Science & Technology**.  

**Certifications:**  
![CompTIA Security+](https://img.shields.io/badge/CompTIA%20Security+-Certified-orange)  

I’m passionate about **defensive and offensive cybersecurity**, building projects that bridge the technical, operational, and strategic aspects of security. My focus is on:

- Threat Detection & Incident Response
- Digital Forensics  
- Secure Systems & Applications  

**Favorite tools:** Autopsy · Python · Kali Linux · Wireshark · Snort  

I’m eager to apply my skills in a professional setting and contribute to real-world cybersecurity solutions while continuing to grow my expertise.  



Cybersecurity Projects:
## Threat Detection & Response
* [Honeypot-Experiment](https://github.com/Aka005/Honeypot-Experiment)

Experimented with deploying honeypots to detect, capture, and analyze network intrusion attempts. Includes automated logging, monitoring, and visualization to study attacker behavior and improve detection capabilities.

## Web & Application Security
* [Jewelry Shop Website](https://github.com/Aka005/IST-256--Jewelry-Shop)

Developed a secure web application using Express.js, Node.js, and MongoDB. Implemented authentication, input validation, and secure REST endpoints to protect user data while demonstrating full-stack security principles.

* [Active Directory project](https://github.com/Aka005/ad-project)

A project focused on building secure, interactive web applications. Implemented front-end and back-end functionality with attention to secure coding practices, input validation, and RESTful APIs.
Personal Portfolio

## Reverse Engineering & Malware Analysis
* [Reverse_Engineering](https://github.com/Aka005/Reverse_Engineering)

Analyzed binaries to understand malware behavior, identify vulnerabilities, and investigate application exploits. Techniques included static and dynamic analysis, improving understanding of threat patterns and reverse engineering methodologies.


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Typing Effect Example</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f4f9;
      color: #333;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }

    h1 {
      font-size: 2.5rem;
      margin: 20px 0;
    }

    .typing {
      border-right: 2px solid #6a0dad;
      white-space: nowrap;
      overflow: hidden;
    }
  </style>
</head>
<body>

  <h1 class="typing" id="aboutMe"></h1>
  <h1 class="typing" id="projects"></h1>

  <script>
    function typeText(elementId, text, speed = 100, callback) {
      let i = 0;
      const el = document.getElementById(elementId);
      function type() {
        if (i < text.length) {
          el.innerHTML += text.charAt(i);
          i++;
          setTimeout(type, speed);
        } else if (callback) {
          callback();
        }
      }
      type();
    }

    // Type "About Me:" then "Cybersecurity Projects:"
    typeText('aboutMe', 'About Me:', 100, () => {
      setTimeout(() => {
        typeText('projects', 'Cybersecurity Projects:', 100);
      }, 500);
    });
  </script>

</body>
</html>
