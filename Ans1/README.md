For security, trivy is one of popular OSS vuln scanning tool. Have scanned nginx:1.19 and nginx:JD1.19 with trivy:

![image1](https://github.com/Jeet-14/CISION/assets/24683251/999d3ab8-4baa-400d-9304-6e8192d67207)


Another build-in tool is scout which can provide details about vulns, 

![image2](https://github.com/Jeet-14/CISION/assets/24683251/79607182-b7d8-407c-b364-dd14a2d7ea3f)

base image nginx:1.19 has more vulns, newly created image JD1.19 has significant less no of vulns and those are non-fixable.
