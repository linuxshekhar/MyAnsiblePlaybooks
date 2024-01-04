# MyAnsiblePlaybooks
Some Ansible Playbooks

<br />
<div align="center">
  <h2 align="center">ARGO JAVA Template</h2>
  <h4 align="center">This repository is template repository for argo-java type jobs.</h4>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#initialinformation">Initial Information</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contribution">Contribution</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## Initial Information
- Base image is variable, for now it support Java version 17 and we can add additional image to artifactory to support different Java versions.
- By default, below listed pacakges are already installed: 
-- bash curl ca-certificates coreutils

### Built With

* [![Argo][Argo.js]][Argo-url]
* [![Java][Java.js]][Java-url]

## Usage
Job Input Variables:
  - **java_version**: As of now, Java 17 is supported.
  - **product-name**: it should be written as single string and in lower case letters. For example 'nebula', 'onepay', 'modern-pip'.
  - **application-name**: it should be single string lower-case name assigned to application, for example 'argo-java-build-test'
  - **built-image** will be available at: ```artifactory.cdk.com/docker-local/<-product-name->/<-application-name->:<-branch-name->.<-githib-runner-id->```

## Contribution

Contributions are always welcome as it will make this template more robust. Any contributions you make are **greatly appreciated**.

To contribute to this repository, you can simply follow below steps:

1. Fork the Project
2. Create your Feature Branch (`git checkout -b <Branch Name>`)
3. Commit your Changes (`git commit -m 'Add some changes'`)
4. Push to the Branch (`git push origin`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

[Orchestration Team](IOPSAutomation@cdk.com)

[CDK Global](https://www.cdkglobal.com)

[![LinkedIn][linkedin-shield]][linkedin-url]
<p align="right">(<a href="#readme-top">back to top</a>)</p>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
<p align="right">(<a href="#readme-top">back to top</a>)</p>

[CDKurl]: (https://www.cdkglobal.com)
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/company/cdknorthamerica
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/argo-java-job-template.svg?style=for-the-badge
[contributors-url]: https://github.com/cdk-prod/argo-java-job-template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/argo-java-job-template.svg?style=for-the-badge
[forks-url]: https://github.com/cdk-prod/argo-java-job-template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/argo-java-job-template.svg?style=for-the-badge
[stars-url]: https://github.com/cdk-prod/argo-java-job-template/stargazers
[Argo.js]: (https://img.shields.io/badge/argo-FF2D20?style=for-the-badge&logo=argo&logoColor=white)
[Argo-url]: (https://argo-workflows.readthedocs.io/en/latest/)
[Java.js]: (https://img.shields.io/badge/Java-DD0031?style=for-the-badge&logo=java&logoColor=white)
[Java-url]: (https://www.java.com/en/)
