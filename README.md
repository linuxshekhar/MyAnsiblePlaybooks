# MyAnsiblePlaybooks
Some Ansible Playbooks

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/cdk-prod/argo-java-job-template">
    <img src="https://argo-workflows.readthedocs.io/en/latest/assets/logo.png" alt="ArgoLogo" width="80" height="80">
    <img src="https://search.oracle.com/img/java-logo.avif" alt="JavaLogo" width="80" height="80">
  </a>
  <h2 align="center">ARGO JAVA Template</h2>
  <h4 align="center">This repository is template repository for argo-java type jobs.</h4>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#initialinformation">Initial Information</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
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

* [![Argo Workflow][ArgoBadge]][ArgoUrl]
* [![Java][JavaBadge]][JavaUrl]

## Usage
Job Input Variables:
  - **java_version**: As of now, Java 17 is supported.
  - **product-name**: it should be written as single string and in lower case letters. For example 'nebula', 'onepay', 'modern-pip'.
  - **application-name**: it should be single string lower-case name assigned to application, for example 'argo-java-build-test'
  - **built-image** will be available at:
  -- artifactory.cdk.com/docker-local/<-product-name->/<-application-name->:<-branch-name->.<-githib-runner-id->

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

Your Name - [Orchestration Team](IOPSAutomation@cdk.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

![ArgoLogo](https://argo-workflows.readthedocs.io/en/latest/assets/logo.png) 
![ArgoBadge](https://img.shields.io/badge/argo-FF2D20?style=for-the-badge&logo=argo&logoColor=white)
![ArgoUrl](https://argo-workflows.readthedocs.io/en/latest/)
![JavaLogo](https://search.oracle.com/img/java-logo.avif)
![JavaBadge](https://img.shields.io/badge/Java-DD0031?style=for-the-badge&logo=java&logoColor=white)
![JavaUrl](https://www.java.com/en/)
![cdkurl](https://www.cdkglobal.com)
